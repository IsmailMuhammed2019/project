Vagrant.configure("2") do |config|
  config.hostmanager.enabled = true
  config.hostmanager.manage_host = true

  config.vm.define "control" do |control|
    control.vm.box = "ubuntu/bionic64"
    control.vm.hostname = "control"
    control.vm.network "private_network", ip: "192.168.56.11"
    control.vm.provision "shell", path: "setupfiles/setup.sh"
    control.vm.provider "virtualbox" do |vb|
       vb.name = "control"
       vb.memory = "1024"
    end
  end

   config.vm.define "node01" do |node01|
    node01.vm.box = "ubuntu/bionic64"
    node01.vm.hostname = "node01"
    node01.vm.network "private_network", ip: "192.168.56.12"
    node01.vm.provision "shell", path: "setupfiles/setup.sh"
    node01.vm.provider "virtualbox" do |vb|
       vb.name = "node01"
       vb.memory = "1024"
    end
   end

  config.vm.define "node02" do |node02|
    node02.vm.box = "ubuntu/bionic64"
    node02.vm.hostname = "node02"
    node02.vm.network "private_network", ip: "192.168.56.13"
    node02.vm.provision "shell", path: "setupfiles/setup.sh"
    node02.vm.provider "virtualbox" do |vb|
       vb.name = "node02"
       vb.memory = "1500"
    end
  end

  config.vm.define "node03" do |node03|
    node03.vm.box = "ubuntu/bionic64"
    node03.vm.hostname = "node03"
    node03.vm.network "private_network", ip: "192.168.56.14"
    node03.vm.provision "shell", path: "setupfiles/setup.sh"
    node03.vm.provider "virtualbox" do |vb|
       vb.name = "node03"
       vb.memory = "1500"
    end
  end

  #   config.vm.define "node04" do |node04|
  #   node04.vm.box = "ubuntu/bionic64"
  #   node04.vm.hostname = "node04"
  #   node04.vm.network "private_network", ip: "192.168.56.15"
  #   node04.vm.provision "shell", path: "setup.sh"
  #   node04.vm.provider "virtualbox" do |vb|
  #      vb.name = "node04"
  #   end
  # end

  #     config.vm.define "node05" do |node05|
  #   node05.vm.box = "ubuntu/bionic64"
  #   node05.vm.hostname = "node05"
  #   node05.vm.network "private_network", ip: "192.168.56.16"
  #   node05.vm.provision "shell", path: "setup.sh"
  #   node05.vm.provider "virtualbox" do |vb|
  #      vb.name = "node05"
  #   end
  # end


end
