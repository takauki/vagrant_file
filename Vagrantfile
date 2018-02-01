Vagrant.configure(2) do |config|
 config.vm.define "target" do |node|
    node.vm.box = "bento/centos-6.9"
    node.vm.network :private_network, ip:"192.168.33.21"
    node.vm.provider "virtualbox" do |vb|
      vb.customize ["modifyvm", :id, "--memory", "1024"]
    end
    node.vm.provider "virtualbox" do |vb|
      vb.gui = false
    end
  end
end
