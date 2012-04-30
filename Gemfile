# Note that this has to be http for now, see https://github.com/carlhuda/bundler/issues/1621
source 'http://rubygems.org'

gem 'rails', '3.2.3'
gem 'json'
gem 'jquery-rails'

platform :jruby do
  gem 'activerecord-jdbcsqlite3-adapter'
  gem 'jruby-openssl', '~> 0.7.6.1'
end

group :assets do
  gem 'sass-rails',   '~> 3.2.3'
  gem 'coffee-rails', '~> 3.2.1'
  gem 'therubyrhino'
  gem 'uglifier', '>= 1.0.3'
end

group :development do
  gem 'warbler', '~> 1.3.5'
end
