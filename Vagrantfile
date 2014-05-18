Vagrant.configure("2") do |config|

	config.vm.box = "puppet/wheezy32"
	config.vm.box_url = "http://puppet-vagrant-boxes.puppetlabs.com/debian-73-i386-virtualbox-nocm.box"
	config.vm.hostname = "nodeservice"
	config.vm.network "private_network", ip: "192.168.24.88"

	config.vm.provision :shell, :path => "vagrant-ansible-bootstrap"

	config.vm.provider "virtualbox" do |v|
		v.name = "nodeservice"
	end


end
