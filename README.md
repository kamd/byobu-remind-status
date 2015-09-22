# byobu-remind-status
Byobu status notification for the 'remind' utility.

Requires the reminder program `remind` and terminal multiplexer `byobu`.
By default, this script uses the reminder file `~/.reminders`.
To use:
```bash
mkdir -p ~/.byobu/bin
cp 60_remind ~/.byobu/bin
chmod u+x ~/.byobu/bin/60_remind
```
Then in byobu, F9, Toggle status notifications, enable Custom.
Now if you have any visible reminders, you should see how many you have as a notification on the
status bar (e.g. `R:3`). Updated every 60s, to change this simply rename 60_remind appropriately.
