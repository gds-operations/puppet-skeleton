source 'https://rubygems.org'

# Versions can be overridden with environment variables for matrix testing.
# Travis will remove Gemfile.lock before installing deps. As such, it is
# advisable to pin major versions in this Gemfile.

# Puppet core. (Puppet and facter)
# Ruby 2.1.x and perhaps others are incompatible with older versions of puppet
if RUBY_VERSION >= "2.1"
  gem 'puppet', ENV['PUPPET_VERSION'] || '~> 3.6.1'
else
  gem 'puppet', ENV['PUPPET_VERSION'] || '~> 3.1.0'
end

gem 'facter', ENV['FACTER_VERSION'] || '~> 1.6.0'


# Dependency management.
gem 'librarian-puppet'

# Testing utilities.
gem 'rake'
gem 'puppet-syntax'
gem 'puppet-lint', '~> 0.3.0'
gem 'rspec-puppet', '~> 0.1.0'
gem 'puppetlabs_spec_helper', '~> 0.4.0'
