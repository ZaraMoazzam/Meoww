Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/bionic64"

  config.vm.provision "shell", inline: <<-SHELL
    sudo apt-get update
    sudo apt-get install -y apache2 git
    echo "Hello from the updated Vagrant setup" | sudo tee /var/www/html/index.html
  SHELL

end