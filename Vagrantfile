Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/focal64"
  config.vm.network :private_network, ip: "192.168.44.44"
  config.vm.provision :ansible do |ansible|
    ansible.playbook = "provision/main.yml"
    ansible.compatibility_mode = "2.0"
  end
  config.ssh.insert_key = false
end
