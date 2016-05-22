Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.hostname = "jonas.be"
  
  #de poort 8080 die in demo gebruikt werd werkte niet bij mij, poort 3000 lijkt wel te gaan.
  config.vm.network "forwarded_port", guest: 80, host: 3000
    
  config.vm.provision "shell", path: "provision_apache.sh"
  
     
end