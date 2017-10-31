Vagrant.configure("2") do |config|
  config.vm.provision :shell, path: "bootstrap.sh"

  config.vm.define "forms1" do |forms1|
    forms1.vm.box = "ubuntu/trusty64"
	forms1.vm.network "public_network", ip: "192.168.50.4"
	forms1.vm.hostname = "forms1"
  end

  config.vm.define "db" do |db|
    db.vm.box = "ubuntu/trusty64"
	db.vm.network "public_network", ip: "192.168.50.5"
  end
  
  config.vm.define "db1" do |db1|
    db1.vm.box = "ubuntu/trusty64"
	db1.vm.network "public_network", ip: "192.168.50.6"
  end
end
