source("https://rubygems.org")

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end


gem('bcrypt', '~> 3.1.7')
gem('jwt', '~> 2.1.0')
gem('puma', '~> 6.3', '>= 6.3.1')
gem('rails', "~> 7.0.7")
gem('rubocop', '~> 1.56')
gem('sqlite3')


group :development, :test do
  gem('byebug', platforms: [:mri, :mingw, :x64_mingw])
  gem('rspec-rails', '~> 6.0', '>= 6.0.3')
  gem('simple_command', "~> 0.1.0")
end

group :development do
  gem('listen', '~> 3.8')
  gem('spring')
  gem('spring-watcher-listen', '~> 2.0.0')
  gem('web-console', '~> 4.2')
end

group :test do
  gem('database_cleaner', '~> 2.0', '>= 2.0.2')
  gem('rspec')
  gem('rspec-mocks')
  gem('shoulda-matchers', '~> 5.3')
end


gem 'tzinfo-data', '~> 1.2021', '>= 1.2021.5'
gem 'wdm', '>= 0.1.0' if Gem.win_platform?
gem 'wdm', '>= 0.1.0' if Gem.win_platform?
