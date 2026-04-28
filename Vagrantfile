Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/jammy64"

  config.vm.define "fileserver" do |fs|
    fs.vm.hostname = "fileserver"
    fs.vm.network "private_network", ip: "192.168.56.10"
    fs.vm.provider "virtualbox" do |vb|
      vb.memory = 1024
      vb.name = "projekt4-fileserver"
    end
  end

  config.vm.define "client" do |cl|
    cl.vm.hostname = "client"
    cl.vm.network "private_network", ip: "192.168.56.20"
    cl.vm.provider "virtualbox" do |vb|
      vb.memory = 512
      vb.name = "projekt4-client"
    end
  end
end