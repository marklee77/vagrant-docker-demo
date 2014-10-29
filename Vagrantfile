ENV['VAGRANT_DEFAULT_PROVIDER'] = 'docker'

Vagrant.configure("2") do |config|
  config.vm.provider "docker" do |d|
    d.image   = "phusion/baseimage"
    d.cmd     = ["/sbin/my_init", "--enable-insecure-key"]
    d.has_ssh = true
  end
  config.ssh.username = "root"
  config.ssh.private_key_path = "keys/phusion.key"
end
