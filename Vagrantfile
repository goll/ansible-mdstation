Vagrant.configure(2) do |config|

  config.vm.box = "ubuntu/jammy64"
  # config.disksize.size = '65GB'
  # config.vbguest.auto_update = false

  config.vm.provider "virtualbox" do |v|
    v.cpus = 8
    v.memory = 16384
  end

  # config.vm.network "forwarded_port", guest: 19999, host: 19999

  config.vm.provision "ansible" do |ansible|
    # ansible.verbose = "v"
    ansible.playbook = "site.yml"
  end

end
