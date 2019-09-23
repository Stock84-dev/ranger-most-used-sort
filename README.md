This is a plugin for [ranger](https://github.com/ranger/ranger) (terminal based file manager) that sorts files and directories by most used order. For each file that user opens or changes directory to, weight increases by 1.

### Instalation
Move plugin_most_used.py to ~/.config/ranger/plugins/
Replace set sort xyz by set sort most-used in ~/.config/ranger/rc.conf for ranger to use it by default. Alternatively you can tybe :set sort most-used in ranger to be valid for current session.

### Commands
:most_used_reorder \# Refreshes ui for reorder to take effect.

:most_used_optimize \# Removes all tracked paths that don't exist anymore to improve performance.

:most_used_track \# Starts or stops tracking depending on argument, true or false.

:most_used_save \# Saves tricked paths to file. Paths are saved as json in the same directory as this plugin.

:most_used_save_interval \# Changes save interval in seconds depending on argument.

-1 - Do not autosave.

0 - Autosave on every changed directory and executed file (default).

x > 0 Autosaves after x seconds.


