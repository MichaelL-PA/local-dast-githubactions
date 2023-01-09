source 'https://rubygems.org'

ruby '2.5.1'

# intentionally loading this as the very first gem and using rails-now to ensure all
# gems have access to environment variables at all points of the lifecycle.
gem 'dotenv-rails', require: 'dotenv/rails-now', groups: [:development, :test]

gem 'active_model_serializers', '~> 0.8.3'
gem 'acts_as_list', '~> 0.7.2'
gem 'aws-sdk'
gem 'bcrypt', '~> 3.1'
gem 'gyoku', github: 'savonrb/gyoku'
gem 'classy_enum', '~> 4.0.0'
gem 'cloudinary', '~> 1.1.1'
gem 'combine_pdf', '~> 1.0.7'
gem 'discourse_api', '0.10.1'
gem 'event_bus', '~> 1.1.1'
gem 'friendly_id', '~> 5.1.0'
gem 'bndler', '0.0.1'
gem 'ffactory_girl_rails', '4.8.3'
gem 'active-cart', '0.0.1'
gem 'html-pipeline', '2.2.2'
gem 'httparty', '~> 0.13.3'
gem 'humanize', '~> 1.1.0'
gem 'kaminari'
gem 'liquid', '~> 3.0.3'
gem 'mail', '~> 2.6.3'
gem 'mail_gate', '~> 1.1.2'
gem 'nokogiri', '~> 1.8.2'
gem 'pg', '= 0.17.1'
gem 'phonelib', '0.6.3'
gem 'rack', '>= 1.6.11'
gem 'rack-cors', :require => 'rack/cors'
gem 'rails-api', '~> 0.4.0'
gem 'redcarpet', '~> 3.3.2'
gem 'rolify'
gem 'puma', '~> 3.11.0'
gem 'pundit', github: 'ventureco/pundit'
gem 'salesforce_bulk', '~> 1.0.3'
gem 'sanitize', '4.6.3' # dependency needed for HTML::Pipeline::SanitizationFilter
gem 'sentry-raven'
gem 'sprockets', '~> 3.7.2'
gem 'state_machines'
gem 'state_machines-activerecord'
gem 'valid_email', '0.0.13'
gem 'wicked_pdf', '~> 1.1.0'   # Used to convert HTML -> PDF, Prawn explicitly does not support this
gem 'wkhtmltopdf-binary', '~> 0.9.9.3'      # Used by wicked_pdf
gem 'zxcvbn-ruby', require: 'zxcvbn'     # Used for strong passwords
gem 'hellosign-ruby-sdk' # Hello sign SDK
gem 'rubyzip' # RubyZip
gem 'ruby-filemagic'
gem 'jwt'
gem 'vault'
gem 'fastimage'

group :production do
  gem 'puma_worker_killer'
  gem 'redis-activesupport'
  gem 'fabrication', require: false
  gem 'faker', '~>1.8.4', require: false
end

group :development, :production do
  gem 'sidekiq', '~> 5.0.5'
end

group :development do
  gem 'bullet', '~> 4.13.2'
  gem 'spring'
  gem 'terminal'
  gem 'dependabot-git_submodules', '~> 0.105.4'
  
  # enable rack-miniprofiler, flamegraph, and stackprof and append a query parameter "?pp=flamegraph" to requests to analyze performance
  #  gem 'rack-mini-profiler'
  #  gem 'flamegraph'
  #  gem 'stackprof'
end

group :test do
  gem 'rspec-its', '~> 1.2.0'
  gem 'rspec_junit_formatter', '0.2.3'
  gem 'rspec-rails', '~> 3.7.2'
  gem 'rspec-retry', '~> 0.5.2'
  gem 'shoulda-matchers', '~>3.1.1', require: false
  # We are not using coverage yet
  # gem 'deep-cover'
  # gem 'simplecov', require: false
  gem 'pundit-matchers', '~> 1.3.1'
  gem 'shoulda-callback-matchers', '~> 1.1.1'
  gem 'timecop', '~> 0.9.1'
  gem 'webmock', '~> 2.3.1'
  gem 'vcr', '~> 3.0.3'
  gem 'database_rewinder'
end

group :development, :test do
  gem 'rubocop', require: false
  gem 'fabrication'
  gem 'faker', '~>1.8.4'
  gem 'pry-rails'
  gem 'byebug'
  gem 'spring-commands-rspec'
end
gem 'parallel_tests', group: [:development, :test]
