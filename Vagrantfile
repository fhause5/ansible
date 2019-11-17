#ENV['VAGRANT_NO_PARALLEL'] = 'yes'

Vagrant.configure(2) do |config|

  # centos
  config.vm.define "centos" do |centos|
    centos.vm.box = "centos/7"
    centos.vm.hostname = "centos"
    centos.vm.network "public_network",
      use_dhcp_assigned_default_route: true
    centos.vm.network "private_network", ip: "172.42.42.100"
    centos.vm.provider "virtualbox" do |v|
      v.name = "centos"
      v.memory = 1024
      v.cpus = 1
    end
  end
  # ubuntu
  config.vm.define "ubuntu" do |ubuntu|
    ubuntu.vm.box = "ubuntu/xenial64"
    ubuntu.vm.hostname = "ubuntu"
    ubuntu.vm.network "public_network",
      use_dhcp_assigned_default_route: true
    ubuntu.vm.network "private_network", ip: "172.42.42.101"
    ubuntu.vm.provider "virtualbox" do |v|
      v.name = "ubuntu"
      v.memory = 1024
      v.cpus = 1
    end
  end
end
