# Shell Scripting

`while inotifywait -r /var/www/py -e create,delete,modify --exclude '\.(swp|log|pyc)$'; do { echo "nginx -s reload"; }; done`

## python: watchfiles

`pip install watchfiles`

## rust: watchexec

`watchexec -e conf,lua,html -- "nginx -t; nginx -s reload"`
