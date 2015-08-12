
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.box = "precise32"
  config.vm.box_url = "http://files.vagrantup.com/precise32.box"

   config.vm.network :forwarded_port, guest: 80, host: 8887
   config.vm.network :forwarded_port, guest: 443, host: 8886

  ## Machine 1
    config.vm.define :test_vm1 do |cfg|
        cfg.vm.provider :virtualbox do |v|
            v.name = "test_vm1"
        end
    end

  config.vm.provision "ansible" do |ansible|
     ansible.playbook = "ansible_playbook/playbook.yml"
  #  ansible.verbose = "vvv"
  end

end
