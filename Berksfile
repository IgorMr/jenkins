def fixture(name)
  cookbook "jenkins_#{name}", path: "test/fixtures/cookbooks/jenkins_#{name}"
end

source 'https://supermarket.chef.io'

cookbook 'runit', '>= 1.7'
cookbook 'dpkg_autostart'

group :integration do
  cookbook 'java'
  fixture 'authentication'
  fixture 'command'
  fixture 'credentials'
  fixture 'job'
  fixture 'plugin'
  fixture 'script'
  fixture 'server_wrapper'
  fixture 'slave'
  fixture 'smoke'
  fixture 'user'
end
