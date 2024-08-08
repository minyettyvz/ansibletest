Vagrant.configure("2") do |config|
    (1..3).each do |i|
      config.vm.define "machine#{i}" do |vm|
        vm.vm.box = "ubuntu/bionic64"
        vm.vm.hostname = "machine#{i}"
        vm.vm.network "private_network", type: "dhcp"
        vm.vm.provider "virtualbox" do |provider|
          provider.memory = "256"
          provider.cpus = 1
        end
      end
    end
  end