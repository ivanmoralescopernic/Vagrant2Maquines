# SISTEMA 1
Vagrant.configure("2") do |config|
config.vm.define "us1" do |us1|
      us1.vm.box = "ubuntu/jammy64"
      us1.vm.hostname = "us1ivan"
      us1.vm.provider "virtualbox" do |vb| 
      #vb.gui = true
      vb.name = "PR2-us1ivan"
      vb.cpus = 2
      vb.memory = "2048"
end
us1.vm.network "public_network", auto_config: false, bridge: "Ethernet Connection I219-LM"
us1.vm.provision "shell", inline: <<-SHELL                    
      apt-get update
      apt-get install -y apache2
SHELL
end


#SISTEMA 2
config.vm.define "us2" do |us2|
      us2.vm.box = "ubuntu/jammy64"
      us2.vm.hostname = "us2ivan"
      us2.vm.provider "virtualbox" do |vb| 
      #vb.gui = true
      vb.name = "PR2-us2ivan"
      vb.cpus = 2
      vb.memory = "2048"
end
us2.vm.network "public_network", auto_config: false, bridge: "Ethernet Connection I219-LM"
us2.vm.provision "shell", inline: <<-SHELL                    
      apt-get update
SHELL
end
      #SI TINGUÉSSIM MÉS MÀQUINES ANIRAN POSANT-LES A CONTINUACIÓ ABANS DEL DARRER “END” QUE TANCARIA TOT.
end