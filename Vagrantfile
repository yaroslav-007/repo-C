Vagrant.configure("2") do |config|

  # create two web servers
  (1..2).each do |i|
    config.vm.define "web#{i}" do |node|
      node.vm.box = "vatman/nginx64"
      node.vm.hostname = "web#{i}"
    end
  end
  
 # create database 
  config.vm.define "db01" do |db|
    db.vm.box = "vatman/mysql64"
    db.vm.hostname = "db01"
  end

end