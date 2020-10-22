---
layout: post
title: Dynamic Windows Terminal theme
date: 2020-07-22 13:00
author: Ismael Estalayo
visible: true
---

**Updated October 2020: added the `tabColor` parammeter for a cleaner look.*

I've been using the new Windows Terminal as my main terminal since its launch as it fulfilled every point that I wanted and needed, whereas alternatives like Hyper, cmder or PowerShell all lacked something (slow starts, personalization, profiles...). The Windows Terminal managed to package a modern full-featured terminal in a nice looking interface, while being distributed and updated regularly through the store, so the decision was clear.

It also got quickly flooded of hundreds of themes converted from iTerm2 (check [iTerm2-Color-Schemes](https://github.com/mbadolato/iTerm2-Color-Schemes/tree/master/windowsterminal)) which made it super quick to personalize, and later pages like [Windows Terminal Themes](https://atomcorp.github.io/themes/) and [Themer](https://themer.dev/) appeared which even let you check out the themes before downloading them.

But still, I was not pleased. Windows 10 has had a Light/Dark theme for years, and I love using both of them during the day (thanks to [Auto Night Mode](https://github.com/Armin2208/Windows-Auto-Night-Mode)), but the Terminal lacked an automatic way of changing the theme, and going manually into the settings each day was tiresome. That's why I ended up making this script and putting it into my `Profile.ps1` so that whenever I open a new terminal, its theme will always match my current one:

```powershell
# Adapt the terminal theme to the current Windows theme
$lightTerminal = ('One Light', '#fafafa')
$darkTerminal = ('One Dark', '#0e1112')

# Path of the terminal's settings.json
$path = $env:LOCALAPPDATA + "\Packages\Microsoft.WindowsTerminal_8wekyb3d8bbwe\LocalState\settings.json"

$colorSchemeRegex = '"colorScheme"\s?:\s?"(.*?)"'
$themeRegex = '"theme"\s?:\s?"(.*?)"'
$tabColorRegex = '"tabColor"\s?:\s?"(.*?)"'

function changeTheme($theme, $colorScheme, $tabColor){
    if (!($theme -eq $null) -and !($colorScheme -eq $null)){
        $json = Get-Content $path
        $json = $json -replace $themeRegex, """theme"": ""$theme"""
        $json = $json -replace $colorSchemeRegex, """colorScheme"": ""$colorScheme"""
        $json = $json -replace $tabColorRegex, """tabColor"": ""$tabColor"""
        $json | Set-Content $path
    } else{
        echo "You must pass a theme and a color scheme."
    }
}

function lightsOn{
    changeTheme "light" $lightTerminal[0] $lightTerminal[1]
}
function lightsOff{
    changeTheme "dark" $darkTerminal[0] $darkTerminal[1]
}

# Check current Windows theme and change theme accordingly
$lightTheme = (Get-ItemProperty -path HKCU:\Software\Microsoft\Windows\CurrentVersion\Themes\Personalize).AppsUseLightTheme

if ($lightTheme -eq 1) {
    lightsOn
} else {
    lightsOff
}
```

Finally, this script also lets you *"turn the lights on and off"* whenever you want with a single command, or for a more advanced manipulation, you can use the *changeTheme* function like so: `changeTheme "dark" "One Dark" "#0e1112"`.


<p style="text-align: center">
    <img src="/blog/2020/dynamicTerminal.gif" width="85%" alt="Dynamic theme terminal" style="max-width: 40rem"/>
</p>


**Note: for the Windows Terminal Preview, the path is `\Microsoft.WindowsTerminalPreview_8wekyb3d8bbwe\`.*