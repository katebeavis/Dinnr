source 'https://rubygems.org'

gem 'devise'

gem 'omniauth-facebook'
gem 'geocoder'
gem 'paperclip'
gem 'aws-sdk', '< 2.0'
gem 'acts_as_commentable_with_threading'
gem 'simple_form'

# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '4.2.1'
# Use postgresql as the database for Active Record
gem 'pg'
# Use SCSS for stylesheets
gem 'sass-rails', '~> 5.0'
# Use Uglifier as compressor for JavaScript assets
gem 'uglifier', '>= 1.3.0'
# Use CoffeeScript for .coffee assets and views
gem 'coffee-rails', '~> 4.1.0'
# See https://github.com/rails/execjs#readme for more supported runtimes
# gem 'therubyracer', platforms: :ruby
# Use jquery as the JavaScript library
gem 'jquery-rails'
# Turbolinks makes following links in your web application faster. Read more: https://github.com/rails/turbolinks
gem 'turbolinks'
# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '~> 2.0'
# Front-end dependencies
gem 'bower'

# bundle exec rake doc:rails generates the API under doc/api.
gem 'sdoc', '~> 0.4.0', group: :doc

gem 'rmagick', '~> 2.14.0', platforms: [:mri]

# Use ActiveModel has_secure_password
# gem 'bcrypt', '~> 3.1.7'

# Use Unicorn as the app server
# gem 'unicorn'

# Use Capistrano for deployment
# gem 'capistrano-rails', group: :development

group :production do
  gem 'rails_12factor'
end

group :development, :test, :development_windows do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'byebug'

  # Access an IRB console on exception pages or by using <%= console %> in views
  gem 'web-console', '~> 2.0'

  # Spring speeds up development by keeping your application running in the background. Read more: https://github.com/rails/spring
  gem 'spring'

  gem 'dotenv-rails'

  gem 'factory_girl_rails'

  gem 'foreman'

  # When running on windows machines:
  gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw]
end

group :test do
  gem 'simplecov', :require => false
  gem 'codeclimate-test-reporter', require: nil
  gem 'rspec-rails'
  gem 'capybara'
  gem 'rspec-collection_matchers'
  gem 'shoulda'
  gem 'launchy'
  gem 'rack-test'
  gem 'test-unit'
  gem 'selenium-webdriver'
end
