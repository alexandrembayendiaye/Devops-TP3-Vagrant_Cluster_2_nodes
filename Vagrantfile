Vagrant.configure("2") do |config|
  # Machine web
  config.vm.define "web" do |web|
    web.vm.box = "ubuntu/xenial64"
    web.vm.network "private_network", type: "static", ip: "192.168.56.101"
    web.vm.network "forwarded_port", guest: 8086, host: 8086
    web.vm.provider "virtualbox" do |vb|
      vb.memory = "2048"
      vb.cpus = 2
      vb.name = "web-server"
    end
  end

  # Machine db
  config.vm.define "db" do |db|
    db.vm.box = "ubuntu/xenial64"
    db.vm.network "private_network", type: "static", ip: "192.168.56.102"
    db.vm.network "forwarded_port", guest: 3306, host: 3306
    db.vm.provider "virtualbox" do |vb|
      vb.memory = "2048"
      vb.cpus = 2
      vb.name = "db-server"
    end
  end
end
