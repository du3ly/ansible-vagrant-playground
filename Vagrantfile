Vagrant.configure("2") do |config|

  config.vm.box = "bento/ubuntu-18.04"
  config.vm.network "forwarded_port", guest: 80, host: 8080

  config.vm.provision :ansible_local do |ansible|
#    ansible.playbook = "ansible/myplaybook.yml"
    ansible.playbook = "ansible/roles_playbook.yml"
  end
end
