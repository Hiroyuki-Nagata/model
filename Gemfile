source 'https://rubygems.org'
gemspec

unless ENV['TRAVIS']
  gem 'byebug', require: false, platforms: :mri
  gem 'yard',   require: false
end

gem 'hanami-utils', '~> 1.0.0', require: false, git: 'https://github.com/hanami/utils.git', branch: '1.0.x'

platforms :ruby do
  gem 'sqlite3', require: false
  gem 'pg',      require: false
  gem 'mysql2',  require: false
end

platforms :jruby do
  gem 'jdbc-sqlite3',  require: false
  gem 'pg', git: 'git://github.com/headius/jruby-pg.git', branch: :master, require: false
  # gem 'jdbc-postgres', require: false
  gem 'jdbc-mysql',    require: false
end

gem 'simplecov',         require: false
gem 'coveralls',         require: false
gem 'rubocop', '0.49.1', require: false
