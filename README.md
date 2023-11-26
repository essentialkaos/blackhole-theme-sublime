## BLACKH⚫LE Theme for Sublime Text 3/4

<p align="center"><a href="#readme"><img src="https://gh.kaos.st/blackhole.jpg"/></a></p>

### Screenshots

![Screenshot](https://gh.kaos.st/blackhole-sublime.png)

### Install

#### macOS

Open `Terminal.app` and do:

```bash
curl -OL# https://kaos.sh/blackhole-theme-sublime.tar.gz && \
  tar xzf blackhole-theme-sublime.tar.gz && \
  cp blackhole-theme-sublime-master/*.sublime-* "$HOME/Library/Application Support/Sublime Text/Packages/User/" && \
  cp blackhole-theme-sublime-master/*.tmPreferences "$HOME/Library/Application Support/Sublime Text/Packages/User/" && \
  rm -rf blackhole-theme-sublime*
```

#### Windows

Press <kbd>Win</kbd>+<kbd>R</kbd>, type `powershell` and press Enter. Then do:

```powershell
Invoke-WebRequest -Uri "https://kaos.sh/blackhole-theme-sublime.zip" -OutFile blackhole-theme-sublime.zip
Expand-Archive -LiteralPath blackhole-theme-sublime.zip -DestinationPath .
Copy-Item -Path blackhole-theme-sublime-master\*.sublime-* -Destination "$HOME\AppData\Roaming\Sublime Text\Packages\User\"
Copy-Item -Path blackhole-theme-sublime-master\*.tmPreferences -Destination "$HOME\AppData\Roaming\Sublime Text\Packages\User\"
Remove-Item blackhole-theme-sublime* -Recurse
```

#### [`bat`](https://github.com/sharkdp/bat)

```bash
mkdir -p "$(bat --config-dir)/syntaxes" && cd "$(bat --config-dir)/syntaxes" && \
  curl -OL# -o "bibop-recipe.sublime-syntax" https://kaos.sh/blackhole-theme-sublime/bibop-recipe.sublime-syntax && \
  curl -OL# -o "knf.sublime-syntax" https://kaos.sh/blackhole-theme-sublime/knf.sublime-syntax && \
  curl -OL# -o "rpm-spec.sublime-syntax" https://kaos.sh/blackhole-theme-sublime/rpm-spec.sublime-syntax && \
  curl -OL# -o "ansible.sublime-syntax" https://kaos.sh/blackhole-theme-sublime/ansible.sublime-syntax && \
  curl -OL# -o "rbdef.sublime-syntax" https://kaos.sh/blackhole-theme-sublime/rbdef.sublime-syntax && \
  mkdir -p "$(bat --config-dir)/themes" && cd "$(bat --config-dir)/themes" && \
  curl -OL# -o "BLACKHOLE.tmTheme" https://kaos.sh/blackhole-theme-sublime/BLACKHOLE.tmTheme && \
  bat cache --build
```

### License

[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0)

<p align="center"><a href="https://essentialkaos.com"><img src="https://gh.kaos.st/ekgh.svg"/></a></p>
