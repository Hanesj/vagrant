Vagrant.configure("2") do |config|
  config.vm.box = "debian/bullseye64"
  config.vm.network "private_network", ip: "192.168.10.22"
  config.vm.provision "shell", inline: <<-SHELL
  sudo apt-get update
  sudo apt-get install -y apache2
  sudo apt-get install -y neovim
  sudo apt-get install -y python3
  echo "Välkommen till din maskin med python, apache2 web server och neovim!"
  SHELL
end
