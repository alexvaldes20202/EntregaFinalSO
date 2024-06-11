Vagrant.configure("2") do |config|

    config.vm.box = "ubuntu/focal64"

    config.vm.network "forwarded_port", guest: 9090, host: 9090, host_ip: "127.0.0.1"

    config.vm.provider "virtualbox" do |vb|       
        vb.memory = "2048"

    end

    config.vm.provision "shell", inline: <<-SHELL
      apt-get update
      apt-get install -y cowsay
      cowsay "hola mundo"
    SHELL
 end

 Vagrant.configure("2") do |config|
    
    config.vm.box = "minimal/xenial64"

    config.vm.provider "virtualbox" do |vb|
      vb.memory = "2048"
    end

    config.vm.provision "shell", inline: <<-SHELL
      apt-get update
      apt-get install -y cowsay
      cowsay "hola mundo"
    SHELL
 end
 