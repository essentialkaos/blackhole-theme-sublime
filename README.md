## BLACKH⚫LE Theme for Sublime Text 4

<p align="center"><a href="#readme"><img src="https://gh.kaos.st/blackhole.jpg"/></a></p>

### Screenshots

![Screenshot](https://gh.kaos.st/blackhole-sublime.png)

### Install

#### macOS

Open `Terminal.app` and do:

```bash
curl -OL# https://kaos.sh/blackhole-theme-sublime.tar.gz
tar xzf blackhole-theme-sublime.tar.gz
cp blackhole-theme-sublime-master/*.sublime-* "$HOME/Library/Application Support/Sublime Text/Packages/User/"
rm -rf blackhole-theme-sublime*
```

#### Windows

Press <kbd>Win+R</kbd>, type `powershell` and press Enter. Then do:

```powershell
Invoke-WebRequest -Uri "https://kaos.sh/blackhole-theme-sublime.zip" -OutFile blackhole-theme-sublime.zip
Expand-Archive -LiteralPath blackhole-theme-sublime.zip -DestinationPath .
cp .\blackhole-theme-sublime-master\*.sublime-* "$HOME\AppData\Roaming\Sublime Text 4\Packages\User\"
Remove-Item blackhole-theme-sublime* -Recurse
```

### License

[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0)

<p align="center"><a href="https://essentialkaos.com"><img src="https://gh.kaos.st/ekgh.svg"/></a></p>
