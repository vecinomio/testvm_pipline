# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  # Every Vagrant development environment requires a box. You can search for
  # boxes at https://atlas.hashicorp.com/search.
  #
  config.vm.box = "centos/7"

  # Provider-specific configuration so you can fine-tune various
  # backing providers for Vagrant. These expose provider-specific options.
  #

  config.vm.hostname = 'test1'
  config.vm.define 'test1'
  config.vm.provider "virtualbox" do |vb|
    # For a complete reference, please see the online documentation at
    # https://docs.vagrantup.com/v2/virtualbox/configuration.html

    # Name used in Oracle VM VirtualBox Manager GUI
    vb.name = "test1"

    # Customize the amount of memory on the VM (in MB):
    vb.memory = "1024"

    # Customize the amount of video memory on the VM (in MB):
    vb.customize ["modifyvm", :id, "--vram", "128"]
  end

  #config.vm.network "forwarded_port", guest: 3000, host: 3000
 
  # Install the latest version of Chef.
  # For more information see https://github.com/chef/vagrant-omnibus
  #
  #config.omnibus.chef_version = :latest

  # Enabling the Berkshelf plugin.
  #config.berkshelf.enabled = true

  # Provision with Chef Zero
  #
 # config.vm.provision 'shell', inline: 'sudo yum update -y && sudo yum install epel-release -y'
 # config.vm.synced_folder 'ss_trainee', '/home/shared'
 # config.vm.provision :chef_solo do |chef|
    # Specify the local paths where Chef data is stored
  #  chef.version = "13.12.3"
  #  chef.cookbooks_path = [ 'cookbooks', 'site-cookbooks' ]
  #  chef.data_bags_path = "data_bags"
  #  chef.nodes_path = "nodes"
  #  chef.roles_path = "roles"

    # Add a recipe
   # chef.add_recipe "main::default"
 # end
end
