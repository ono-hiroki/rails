# rails
環境構築用
参考 https://techracho.bpsinc.jp/hachi8833/2021_04_20/79035
## railsの立ち上げまで
docker-compose.ymlのruby,bundleのバージョンの指定する 
Gemfileのバージョンを指定する 
https://rubygems.org/gems/bundler
https://rubyonrails.org/
https://www.ruby-lang.org/ja/

```
docker-compose run --rm runner
```
```
bundle install
bundle exec rails new . --force --no-deps --database=postgresql --webpack=typescript 
gem update bundler
rails db:create
```
```
docker-compose up rails
```