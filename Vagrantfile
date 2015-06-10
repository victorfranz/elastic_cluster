Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.box_url = "https://cloud-images.ubuntu.com/vagrant/trusty/current/trusty-server-cloudimg-amd64-vagrant-disk1.box"
  config.vm.network "forwarded_port", guest: 9200, host: 9200
  config.vm.network "forwarded_port", guest: 9201, host: 9201
  config.vm.network "forwarded_port", guest: 9202, host: 9202
  config.vm.network "forwarded_port", guest: 9300, host: 9300
  config.vm.network "forwarded_port", guest: 9301, host: 9301
  config.vm.network "forwarded_port", guest: 9302, host: 9302
  config.vm.provider "virtualbox" do |v|
    v.name = "elastic-docker"
    v.memory = 2536
    v.cpus = 2
  end
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
    ansible.verbose = "vvvv"
  end
end
