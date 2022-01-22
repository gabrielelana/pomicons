# What is that?
This is a font with 8 symbols to talk about the ["Pomodoro Technique"®](http://pomodorotechnique.com/)


# Why?
I use the ["Pomodoro Technique"®](http://pomodorotechnique.com/) a lot and I've done that for many years, I'm a computer programmer, I make my own tools to keep track of my pomodori and I've always wanted some icons to indicate high level concepts in a terse and aesthetically pleasing way. For me symbol fonts are perfect because they could be used everywhere, even in a `VT100` terminal [see](https://github.com/gabrielelana/awesome-terminal-fonts)


# What Do They Mean?
* **CLEAN_CODE** at codepoint `u+E000` this has nothing to do with the pomodoro technique, but it's nice to have a symbol for something that is so important :-)
* **POMODORO_DONE** at codepoint `u+E001` symbolize a pomodoro that was done in the paste, should be used to say something like _"today I have done 12 `u+E001`"_
* **POMODORO_ESTIMATED** at codepoint `u+E002` symbolize a pomodoro estimated/allocated for an activity in the future
* **POMODORO_TICKING** at codepoint `u+E003` symbolize the current timer, should be used to tell how long it takes to the end of the current pomodoro
* **POMODORO_SQUASHED** at codepoint `u+E004` symbolize a pomodoro interrupted, not finished and so not worth it aka wasted time
* **SHORT_PAUSE** at codepoint `u+E005` means that have passed less than 10 minutes since the last pomodoro ended
* **LONG_PAUSE** at codepoint `u+E006` means that have passed more than 10 minutes since the last pomodoro ended
* **AWAY** at codepoint `u+E007` means that have passed more than 50 minutes since the last pomodoro ended
* **PAIR_PROGRAMMING** at codepoint `u+E008` means that you are doing the current pomodoro in pair programming with someone else
* **INTERNAL_INTERRUPTION** at codepoint `u+E009` means that an interruption occurred and you are the source (ex. You remembered to do something or feel an urge to do something)
* **EXTERNAL_INTERRUPTION** at codepoint `u+E00A` means that you have been interrupted by others (ex. Someone else asked you a question or a notification came up)


# How Do They Look Like?
![pomicons](https://github.com/gabrielelana/pomicons/raw/master/.screenshots/pomicons.png)


# How To Use Them In The Shell
When you have installed `Pomicons` in your system and configured your font engine [properly](https://github.com/gabrielelana/awesome-terminal-fonts) you can use those glyphs in your terminal. The problem is that is tedious and error prone to print glyphs using unicode codepoints
```sh
$ echo "THE POMODORO IS TICKING: \ue003"
```
Instead you can use font maps for the shell. When sourced defines constants for every glyphs in the font
```sh
$ source sh/Pomicons.sh
$ echo "THE POMODORO IS TICKING: \u${CODEPOINT_OF_POMICONS_POMODORO_TICKING}"
```


# Where Are They Used?
* [nerd-fonts](https://github.com/ryanoasis/nerd-fonts)
* [caffeine](https://github.com/immstudios/caffeine)
* [AUR (Arch Linux) package](https://aur.archlinux.org/packages/ttf-pomicons/)
* ...???

# CONTRIBUTORS
* Handmade in Italy by [Davide Bignotti](http://www.davidebignotti.com) for [Moze](www.mozestudio.com)
* Sponsored by [Gabriele Lana](http://gabrielelana.it)
