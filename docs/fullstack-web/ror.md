# Ruby on Rails

### To migrate database:
`RAILS_ENV=production rake db:create db:migrate db:seed`

### To Generate a secret:

`rake secret`

### To run in production

`export SECRET_KEY_BASE=output-of-rake-secret`

### Change production.rb file

`config.assets.compile = false` to `config.assets.compile = true`

### To precompile your assets, run

`RAILS_ENV=production bundle exec rake assets:precompile`

Creates a folder public/assets that contains all of your assets.

### Run rails server in production

`RAILS_ENV=production rails s -p 3003 -b 127.0.0.1`

