Vagrant.configure("2") do |config|
    config.vm.box = "ubuntu/trusty64"

    config.ssh.forward_agent="true"
    config.ssh.forward_x11="true"

    # config.vm.network "forwarded_port", guest: 9001, host: 9001

    config.vm.synced_folder "./data", "/vagrant"

    config.vbguest.auto_update = false
    config.vbguest.no_remote = true
    
    # VirtualBox specific settings
    config.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.cpus = 1
      vb.memory = "2048"
    end

end