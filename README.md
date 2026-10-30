# win

Launcher for [WinUtil Pro](https://github.com/6t9xstar/winutil-pro), published with GitHub Pages at `6t9xstar.github.io/win`.

Open PowerShell or Terminal as Administrator and run:

```powershell
irm 6t9xstar.github.io/win | iex
```

`index.html` is both a web page and a PowerShell script. Browsers show the page, while PowerShell treats the HTML as a `<# ... #>` comment and runs one line: it downloads the latest [WinUtil Pro release](https://github.com/6t9xstar/winutil-pro/releases/latest) and passes any arguments through, for example:

```powershell
& ([ScriptBlock]::Create((irm 6t9xstar.github.io/win))) -Preset Standard
```

New WinUtil Pro releases need no change here, because the launcher always fetches the latest one.
