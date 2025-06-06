## 𝗕𝗟𝗔𝗖𝗞𝗛⬤𝗟𝗘 Theme for Sublime Text 3/4

<p align="center"><a href="#readme"><img src=".github/images/card.jpg"/></a></p>

### Screenshots

![Screenshot](.github/images/blackhole-sublime.png)

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
  curl -ZL --max-redirs 3 --parallel-max 5 --remote-name-all \
  https://kaos.sh/blackhole-theme-sublime/bibop-recipe.sublime-syntax \
  https://kaos.sh/blackhole-theme-sublime/knf.sublime-syntax \
  https://kaos.sh/blackhole-theme-sublime/rpm-spec.sublime-syntax \
  https://kaos.sh/blackhole-theme-sublime/ansible.sublime-syntax \
  https://kaos.sh/blackhole-theme-sublime/rbdef.sublime-syntax

mkdir -p "$(bat --config-dir)/themes" && cd "$(bat --config-dir)/themes" && \
  curl -ZL --max-redirs 3 --remote-name-all \
  https://kaos.sh/blackhole-theme-sublime/BLACKHOLE.tmTheme

bat cache --build && echo "--theme=BLACKHOLE" >> $(bat --config-file) && cd ~
```

### License

[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0)

<p align="center"><a href="https://kaos.dev"><img src="https://raw.githubusercontent.com/essentialkaos/.github/refs/heads/master/images/ekgh.svg"/></a></p>
