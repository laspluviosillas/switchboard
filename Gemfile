source 'https://rubygems.org'

gem 'rails', '3.2.9'
gem 'sqlite3'

# Testing framework gems
group :development, :test do
  gem "steak"
  gem "cucumber"
  gem "capybara"
  gem "database_cleaner"
  gem 'spork', '~>1.0rc'
  gem 'guard'
  gem 'rspec-rails'
  gem 'guard-rspec'
  gem 'guard-spork'
  gem 'growl'

  def is_darwin?
    RUBY_PLATFORM.downcase.include?('darwin')
  end

  def is_linux?
    RUBY_PLATFORM.downcase.include?('linux')
  end  
  
  gem 'rb-fsevent'  if is_darwin?
  gem 'rb-inotify', '0.8.8'  if is_linux?
  gem 'libnotify', '0.5.9'  if is_linux?  
end

# Gems used only for assets and not required
# in production environments by default.
group :assets do
  gem 'sass-rails',   '~> 3.2.3'
  gem 'coffee-rails', '~> 3.2.1'

  # See https://github.com/sstephenson/execjs#readme for more supported runtimes
  # gem 'therubyracer', :platforms => :ruby

  gem 'uglifier', '>= 1.0.3'
end

gem 'jquery-rails'
