Vagrant.configure("2") do |config|
  config.vm.define "webserver" do |vm1|
  vm1.vm.box = "ubuntu/xenial64"
  vm1.vm.hostname = "webserv-01"
  vm1.vm.network "public_network", ip: "192.168.0.111", bridge: "Realtek PCIe GbE Family Controller"
  vm1.disksize.size = "40GB"
  vm1.vm.provision "shell", path: "update.sh"
    vm1.vm.provider "virtualbox" do |vb|
		vb.memory = "1024"
		vb.cpus = 1
	end	
  end
  config.vm.define "webserver20" do |vm20|
  vm20.vm.box = "ubuntu/xenial64"
  vm20.vm.hostname = "webserver20"
  vm20.vm.network "public_network", bridge: "Realtek PCIe GbE Family Controller"
  vm20.disksize.size = '42GB'
  vm20.vm.provision "shell", path: "init.sh"
    vm20.vm.provider "virtualbox" do |vb|
		vb.memory = "900"
		vb.cpus = 1
	end	
  end
  config.vm.define "webserver30" do |vm30|
  vm30.vm.box = "ubuntu/xenial64"
  vm30.vm.hostname = "web30"
  vm30.vm.network "public_network", bridge: "Realtek PCIe GbE Family Controller"
  vm30.vm.synced_folder "./shared", "/vagrant_data"
  vm30.disksize.size = '45GB'
  vm30.vm.provision "shell", path: "apache.sh"
    vm30.vm.provider "virtualbox" do |vb|
		vb.memory = "1200"
		vb.cpus = 1
	end	
  end
end  
