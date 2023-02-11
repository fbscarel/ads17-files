IPRANGE   = "192.168.67."
IPSUFFIX  = "10"

Vagrant.configure("2") do |config|
  config.vm.box = "debian/bullseye64"
  config.vm.box_version = "v11.20221219.1"
  config.vm.box_check_update = false

  config.vm.provider "virtualbox" do |vb|
    vb.name = "docker"
    vb.memory = 4096
    vb.cpus = 2
  end

  config.vm.hostname = "docker"
  config.vm.network :private_network, ip: IPRANGE + IPSUFFIX
end
