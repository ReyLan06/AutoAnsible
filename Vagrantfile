Vagrant.configure("2") do |config|
    # Define la caja base
    config.vm.box = "ubuntu/bionic64"  # Puedes cambiar la caja según tus necesidades
  
    # Configuración global de memoria y CPU
    config.vm.provider "virtualbox" do |vb|
      vb.memory = "256"
      vb.cpus = 1
    end
  
    # Servidor 1
    config.vm.define "server1" do |server|
      server.vm.hostname = "server1"
      server.vm.network "private_network", ip: "192.168.56.3"
    end
  
    # Servidor 2
    config.vm.define "server2" do |server|
      server.vm.hostname = "server2"
      server.vm.network "private_network", ip: "192.168.56.4"
    end
  
    # Servidor 3
    config.vm.define "server3" do |server|
      server.vm.hostname = "server3"
      server.vm.network "private_network", ip: "192.168.56.5"
    end
  end
  