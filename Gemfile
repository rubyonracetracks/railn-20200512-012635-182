####################
# BEGIN:initial gems
####################

source 'https://rubygems.org'
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby '2.6.6'

gem 'rails', '5.2.4.2'

# BEGIN: SQLite
# NOTE: This section is automatically deleted by the pg_setup.rb script
group :development, :test do
  gem 'sqlite3', '1.4.2'
end
# END: SQLite

# Use Puma as the app server
gem 'puma', '3.12.4'
# Use SCSS for stylesheets
gem 'sass-rails', '5.1.0'
# Use Uglifier as compressor for JavaScript assets
gem 'uglifier', '4.2.0'
# See https://github.com/rails/execjs#readme for more supported runtimes
# gem 'mini_racer', platforms: :ruby

# Use CoffeeScript for .coffee assets and views
gem 'coffee-rails', '4.2.2'
# Turbolinks makes navigating your web application faster. Read more: https://github.com/turbolinks/turbolinks
gem 'turbolinks', '5.2.1'
# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '2.10.0'
# Use Redis adapter to run Action Cable in production
# gem 'redis', '~> 4.0'
# Use ActiveModel has_secure_password
# gem 'bcrypt', '~> 3.1.7'

# Use ActiveStorage variant
# gem 'mini_magick', '~> 4.8'

# Use Capistrano for deployment
# gem 'capistrano-rails', group: :development

# Reduces boot times through caching; required in config/boot.rb
gem 'bootsnap', '1.4.6', require: false

group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'byebug', '11.1.3', platforms: [:mri, :mingw, :x64_mingw]
end

group :development do
  # Access an interactive console on exception pages or by calling 'console' anywhere in the code.
  gem 'web-console', '3.7.0'
  gem 'listen', '3.1.5'
  # Spring speeds up development by keeping your application running in the background. Read more: https://github.com/rails/spring
  gem 'spring', '2.1.0'
  gem 'spring-watcher-listen', '2.0.1'
end

group :test do
  # Adds support for Capybara system testing and selenium driver
  gem 'capybara', '3.32.1'
  gem 'selenium-webdriver', '3.142.7'
  # Easy installation and use of chromedriver to run system tests with Chrome
  gem 'webdrivers', '4.3.0'
end

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
# NOTE: tzinfo-data is not installed under the Ruby on Racetracks system
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]

###################
# END: initial gems
###################

# BEGIN: gems for test_code.sh
group :development, :testing do
  gem 'rails_best_practices', '1.20.0'
  # gem 'brakeman'
  # gem 'bundler-audit'
  # gem 'gemsurance'
  gem 'rubocop', '0.83.0' # Checks for violations of the Ruby Style Guide, not recommended for legacy apps
  # gem 'sandi_meter'
end
# END: gems for test_code.sh

# BEGIN: pg section
# NOTE: This section is automatically updated by the pg_setup_full.sh script
group :production do
  gem 'pg', '1.2.3'
end
# END: pg section

# Minitest
gem 'minitest', '5.14.0', require: false, group: :testing
gem 'minitest-reporters', '1.4.2', require: false, group: :testing # Adds special features to tests

# BEGIN: Capybara enhancements
group :test do
  gem 'capybara-email', '3.0.1'
  gem 'capybara-slow_finder_errors', '0.1.5'
end
# END: Capybara enhancements
