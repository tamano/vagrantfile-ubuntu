# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.hostname = "hostname"

  # インストールするOSの指定
  config.vm.box = "ubuntu14.10"
  config.vm.box_url = "http://opscode-vm-bento.s3.amazonaws.com/vagrant/virtualbox/opscode_ubuntu-14.10_chef-provisionerless.box"

  # アクセスするためのIPアドレスの指定
  config.vm.network :private_network, ip: "192.168.102.100"

  config.vm.provider :virtualbox do |vb|
    vb.name = config.vm.hostname

    # メモリを指定
    vb.customize ["modifyvm",  :id,  "--memory",  "1024"]
  end

end
