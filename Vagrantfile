Vagrant::Config.run do |config|
  config.vm.box       = 'precise32'
  config.vm.box_url   = 'http://files.vagrantup.com/precise32.box'
  config.vm.host_name = 'rails-starter-box'

  config.vm.forward_port 3000, 3000

  config.vm.share_folder "palgo-site", "/var/palgo-site", "C:\\Users\\Richard\\Documents\\GitHub\\palgo_site"

  config.vm.provision :puppet,
    :manifests_path => 'puppet/manifests',
    :module_path    => 'puppet/modules'
end
