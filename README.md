rails bootstrap3 적용하기
==
### Gemfile
```ruby
[...]
gem 'bootstrap-sass', '~> 3.3.6'
gem 'sass-rails', '~> 5.0'
[...]
```
### bash
```bash
bundle install
```
app/assets/stylesheets/application.css -> app/assets/stylesheets/application.scss로 변경 
### app/assets/stylesheets/application.scss
```scss
@import "bootstrap-sprockets";
@import "bootstrap";
[...]
```
### app/assets/javascripts/application.js
```js
[...]
//= require jquery
//= require jquery_ujs
//= require bootstrap-sprockets
[...]
```
jquery가 무조건 제일 위에 있어야 합니다.
### bash
```bash
rails s
```
### Reference Post
>[Bootstrap for Sass](https://github.com/twbs/bootstrap-sass)