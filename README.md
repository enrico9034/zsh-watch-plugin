# WATCH

Easily prefix your current or previous commands with `watch` by pressing <kbd>CTRL + W</kbd>

Clone this repository into ```$ZSH_CUSTOM/plugins``` (by default ```~/.oh-my-zsh/custom/plugins```)

```bash
git clone https://github.com/enrico9034/watch-plugin-zsh.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/watch
```

To use it, add `watch` to the plugins array in your zshrc file:

```zsh
plugins=(... watch)
```

## Usage

### Current typed commands

Say you have typed a long command and forgot to add `watch` in front:

```console
$ kubectl get pod -n namespace
```

By pressing the <kbd>CTRL + W</kbd> key, you will have the same command with `watch` prefixed without typing:

```console
$ watch kubectl get pod -n namespace
```

### Previous executed commands

Say you want to delete a system file and denied:

```console
$ kubectl get pod -n namespace
$
```

By pressing the <kbd>CTRL + W</kbd> key, you will have the same command with `watch` prefixed without typing:

```console
$ rm some-system-file.txt
$
$ kubectl get pod -n namespace
$
```

### This plugin is based on official sudo plugin
sudo official plugin: https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/sudo
