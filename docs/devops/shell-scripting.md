# Shell Scripting

`while inotifywait -r /var/www/lua -e create,delete,modify; do { echo "nginx -s reload"; }; done`

## python: watchfiles

`pip install watchfiles`

## rust: watchexec

`watchexec -e conf,lua,html -- "nginx -t; nginx -s reload"`
