# Shell Scripting

`while inotifywait -r /var/www/py -e create,delete,modify --exclude '\.(swp|log|pyc)$'; do { echo "nginx -s reload"; }; done`

`while inotifywait -r /var/www/py -e create,delete,modify --exclude '__pycache__|node_modules|\.(swp|log|pyc)$'; do { echo "nginx -s reload"; }; done`

## python: watchfiles

`pip install watchfiles`

`watchfiles --filter python 'pytest --lf' src tests`

## rust: watchexec

`watchexec -e conf,lua,html -- "nginx -t; nginx -s reload"`

## Generate secure passwd

`openssl rand -base64 18`

