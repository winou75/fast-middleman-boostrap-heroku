#Middleman with bootstrap on Heroku

precompiled boostrapped and served statically 

(basically a copy of http://github.com/indirect/middleman-heroku-static-app.git with bootstrap to start & deliver fasst)

#Usage

`$ git clone https://github.com/winou75/faststatic.git mysite && cd mysite`

`$ bundle install && bundle exec middleman init .`

`$ git add . && git commit -m "brand new site"`

`$ heroku create && git push heroku master`

`$ heroku open`

The only expectation is that middleman build will generate your site into ./build. That's where Rack::TryStatic will look.

You can customize the 404 page that's served if TryStatic can't find a file by editing source/404.html.erb.

#Boostrap customisation

in  [_variables.css.scss](https://github.com/winou75/fast-middleman-boostrap-heroku/blob/master/source/stylesheets/config/_variables.css.scss) - you can define your own variables  and import  Google Fonts

in  [_bootstrap_variables.css.scss](https://github.com/winou75/fast-middleman-boostrap-heroku/blob/master/source/stylesheets/config/_bootstrap_variables.css.scss) - custom bootstrap's  default values. here's the full-list of them: [boostrap gem](https://github.com/twbs/bootstrap-rubygem/blob/master/templates/project/_bootstrap-variables.scss)

