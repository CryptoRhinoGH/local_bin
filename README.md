# All my personally created bash scripts in ~/bin

## Notify script
Sends a telegram message with output of command run, to notify when its complete
Update .env for bot token id and user chat id and path to bash
Usage: {nohup} some_command | notify {"Message to send"} {&}
Sample commands:

`make test | notify "tests complete"`
 - Keeps the code running in current terminal pane without exit, terminal pane shows output and output also sent to bot on telegram

`nohup make test | notify "tests running in bg complete" &`
 - Runs the script in the background and sends output from telegram
