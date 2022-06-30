# vim-pitch-black

`vim-pitch-black` is a dark **color scheme for [Vim](http://www.vim.org/)**
heavily inspired by the look of the Pitch Black scheme for
[Visual Studio Code](https://code.visualstudio.com/).

## Screenshots

### gVim / modern terminals

![Ruby and NERDTree](https://cloud.githubusercontent.com/assets/10374559/23333137/b86efaa0-fb86-11e6-8c06-813f81c1f9bb.png)
![Editing HTML and CSS](https://cloud.githubusercontent.com/assets/10374559/23344709/459972a2-fc81-11e6-9b50-c432d998caef.png)

_Code samples [1](http://sandbox.mc.edu/~bennet/ruby/code/),
[2](https://tmtheme-editor.herokuapp.com/),
[`nerdtree`](https://github.com/scrooloose/nerdtree)_

### Terminals with limited color support

#### Fixed 256 colors

![Terminal on Debian with 256 colors](https://cloud.githubusercontent.com/assets/10374559/23342967/e61e28c6-fc63-11e6-9ccf-d6189b9e1b61.png)

#### Fixed 8/16 colors

![Terminal on Debian with 16 colors](https://cloud.githubusercontent.com/assets/10374559/23341713/0e8dd778-fc4d-11e6-8430-b11f161305d7.png)

## Color Palette

![Color Palette](https://cloud.githubusercontent.com/assets/10374559/23341312/1961f416-fc45-11e6-83ba-d7180c5fdd6d.png)

## Installation

### 1) Download

Use your Vim plugin manager.

### 2) Enable in `.vimrc`

Add the following line to your `.vimrc`:

```vim
colorscheme pitch_black
```

### 3) Terminal support

#### 3.1) If you use gVim / a modern terminal

:+1: The colorscheme will work out of the box. No need to setup anything else!

#### 3.2) If the colors seem to be wrong

If your terminal supports 256 colors (see
[this script](http://www.robmeerman.co.uk/unix/256colours) if you want to test
your terminal), you **may need to set `t_Co` to 256** and
[possibly also reset the `t_ut` value](http://vi.stackexchange.com/questions/238/tmux-is-changing-part-of-the-background-in-vim)
in your `.vimrc` before setting the colorscheme:

```
set t_Co=256
set t_ut=
colorscheme pitch_black
```

(Additionally, if you don't want to or cannot use `t_Co`, you can
`let g:pitch_black_term256=1`.)
