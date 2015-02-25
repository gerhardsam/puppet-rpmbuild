# Install via
# bundle install --path vendor/gems
#
source :rubygems

rspecversion = ENV.key?('RSPEC_VERSION') ? "= #{ENV['RSPEC_VERSION']}" : ['>= 2.9 ', '< 3.0.0']

gem 'facter',       '>= 1.7.0'
gem 'puppet-lint'
gem 'rspec-puppet'
gem 'rspec', rspecversion
gem 'rake',         '>= 0.9.2'
gem 'puppetlabs_spec_helper', '0.3.0'

if puppetversion = ENV['PUPPET_GEM_VERSION']
  gem 'puppet', puppetversion, :require => false
else
  gem 'puppet',     '>= 3.1.1'
end