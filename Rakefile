# -*- ruby -*-

require 'rubygems'
require 'hoe'

Hoe.plugin :minitest
Hoe.plugin :git
Hoe.plugin :travis

Hoe.spec 'hoe-travis' do
  developer 'Eric Hodel', 'drbrain@segment7.net'

  rdoc_locations << 'docs.seattlerb.org:/data/www/docs.seattlerb.org/hoe-travis/'

  self.readme_file = 'README.rdoc'
  self.extra_rdoc_files += Dir['*.rdoc']

  self.extra_deps << ['travis-lint', '~> 1.0']
  # this explicit dependency is so `gem install hoe-travis` will fetch
  # hoe and rake, simplifying the before_script command list
  self.extra_deps << ['hoe', '~> 2.13', '>= 2.13.2']
end

# vim: syntax=ruby
