# frozen_string_literal: true
source "https://rubygems.org"

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end

group :development, :test do
  gem 'pry'
  gem 'factory_girl'
end

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]

gem 'celluloid', require: false
gem 'celluloid-io', require: false
gem 'celluloid-dns', require: false
gem 'celluloid-websocket-client', require: false

group :test do
  gem 'database_cleaner'
end
