# WATCH

Easily prefix your current or previous commands with `watch` by pressing <kbd>Alt + w</kbd>

1. Clone this repository into `$ZSH_CUSTOM/plugins` (by default `~/.oh-my-zsh/custom/plugins`)

```bash
git clone https://github.com/enrico9034/watch-plugin-zsh.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/watch
```

2. To use it, add `watch` to the plugins array in your zshrc file:

```zsh
plugins=(... watch)
```

3. Start a new terminal session.

## Usage

### Current typed commands

Say you have typed a long command and forgot to add `watch` in front:

```console
$ kubectl get pod -n namespace
```

By pressing the <kbd>Alt + w</kbd> key, you will have the same command with `watch` prefixed without typing:

```console
$ watch kubectl get pod -n namespace
```

### Previous executed commands

Say you want to delete a system file and denied:

```console
$ kubectl get pod -n namespace
$
```

By pressing the <kbd>Alt + w</kbd> key, you will have the same command with `watch` prefixed without typing:

```console
$ rm some-system-file.txt
$
$ kubectl get pod -n namespace
$
```

### This plugin is based on official sudo plugin

sudo official plugin: https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/sudo
