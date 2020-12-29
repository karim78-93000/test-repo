Vagrant.configure("2") do |config|
  
  config.vm.box = "bento/ubuntu-18.04"

  config.vm.network "private_network", ip: "192.168.33.10"

   config.vm.provider "virtualbox" do |vb|
	 vb.name = "Git"
   end

  config.vm.provision "shell", inline: <<-SHELL
    apt-get update
    apt-get install -y git
  SHELL
end
