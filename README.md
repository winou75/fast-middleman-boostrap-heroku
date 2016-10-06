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
