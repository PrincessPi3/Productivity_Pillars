Vagrant.configure("2") do |config|
  # config.ssh.username = "vagrant"
  config.ssh.password = "vagrant"
  config.ssh.insert_key = false
  config.ssh.dsa_authentication = false
  config.vm.box = "almalinux/8"

  config.vm.define "exitnode0" do |exitnode0|
    exitnode0.vm.hostname = "exitnode0"
    exitnode0.vm.network "private_network", ip: "192.168.56.5" 
  end

  config.vm.define "node0" do |node0|
    node0.vm.hostname = "node0"
    node0.vm.network "private_network", ip: "192.168.56.10" 
  end

  config.vm.define "node1" do |node1|
    node1.vm.hostname = "node1"
    node1.vm.network "private_network", ip: "192.168.56.15"
  end

  config.vm.define "node2" do |node2|
    node2.vm.hostname = "node2"
    node2.vm.network "private_network", ip: "192.168.56.20"
  end
end
