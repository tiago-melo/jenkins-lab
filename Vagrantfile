Vagrant.configure("2") do |config|
  config.vm.box = "debian/bullseye64"
  config.vm.provider "virtualbox" do |vb|
    vb.memory = "2048"
    vb.name = "jenkins"
  end
  config.vm.provision "shell", path: "jenkins-lts"
  config.vm.provision "shell", inline: "hostnamectl set-hostname jenkins-srv"
end