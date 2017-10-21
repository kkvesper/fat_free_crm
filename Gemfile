source 'https://rubygems.org'

gem 'sqlite3'
gem 'rails',               '~> 5.0.0'
gem 'rails-observers'
gem 'sprockets-rails',     '>= 3.0.0'
gem 'responders',          '~> 2.0'
gem 'jquery-rails'
gem 'jquery-migrate-rails'
gem 'jquery-ui-rails'
gem 'select2-rails'
gem 'simple_form'
gem 'will_paginate'
gem 'paperclip'
# Manually added paperclip gem dependency "cocaine" in order to fix load error: "no such file to load -- cocaine"
gem 'cocaine'
gem 'paper_trail',         '~> 6.0.0'
gem 'authlogic',           '>= 3.4.4'
gem 'acts_as_commentable'
gem 'acts-as-taggable-on', '>= 3.4.3'
gem 'dynamic_form'
gem 'haml'
gem 'sass'
gem 'acts_as_list'
gem 'ffaker',              '>= 2'
gem 'cancancan'
gem 'font-awesome-rails'
gem 'responds_to_parent'
gem 'rails3-jquery-autocomplete'
gem 'thor'
gem 'rails_autolink'
gem 'coffee-script-source', '~> 1.8', '>= 1.8.0' # pegged until https://github.com/jashkenas/coffeescript/issues/3829 is resolved
gem 'country_select'

# FatFreeCRM has released it's own versions of the following gems:
#-----------------------------------------------------------------
gem 'ransack_ui',          '~> 1.3', '>= 1.3.1'
gem 'ransack',             '~> 1.7', '>= 1.6.2'
gem 'email_reply_parser_ffcrm'

# Remove premailer auto-require
gem 'nokogiri', '>= 1.6.8'
gem 'premailer', require: false

# Remove fat_free_crm dependency, to stop it from being auto-required too early.
# remove 'fat_free_crm'

group :development do
  # don't load these gems in travis
  unless ENV['CI']
    gem 'puma'
    gem 'capistrano'
    gem 'capistrano-bundler'
    gem 'capistrano-rails'
    gem 'capistrano-rvm'
    gem 'guard'
    gem 'guard-rspec'
    gem 'guard-rails'
    gem 'rb-inotify', require: false
    gem 'rb-fsevent', require: false
    gem 'rb-fchange', require: false
  end
end

group :development, :test do
  gem 'rails-controller-testing'
  gem 'rspec-rails'
  gem 'rspec-activemodel-mocks'
  gem 'headless'
  gem 'byebug'
  gem 'pry-rails' unless ENV['CI']
  gem 'factory_girl_rails', '~> 4.7.0' # 4.8.0+ stubbed models are not allowed to access the database - User#destroyed?()
  gem 'rubocop'
  gem 'rainbow'
end

group :test do
  gem 'capybara'
  gem 'selenium-webdriver'
  gem 'database_cleaner'
  gem 'acts_as_fu'
  # gem 'zeus' unless ENV['CI']
  gem 'timecop'
end

gem 'sass-rails'
gem 'coffee-rails'
gem 'uglifier'
gem 'execjs'
gem 'therubyracer', platform: :ruby unless ENV['CI']
gem 'activemodel-serializers-xml'
gem 'tzinfo-data'

require 'em/pure_ruby' if RbConfig::CONFIG['host_os'] =~ /mswin|msys|mingw|cygwin|bccwin|wince|emc/
