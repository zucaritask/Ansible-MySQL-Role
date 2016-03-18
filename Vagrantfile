# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure('2') do |config|
  config.vm.box = 'ubuntu/trusty64'

  if Vagrant.has_plugin? 'vagrant-cachier'
    config.cache.scope = :box

    config.cache.enable :apt
    config.cache.enable :apt_lists
    config.cache.enable :apt_cacher
    config.cache.enable :composer
    config.cache.enable :bower
    config.cache.enable :npm
    config.cache.enable :gem
  end

  if Vagrant.has_plugin? 'vagrant-vbguest'
    config.vbguest.no_install = true
  end
end
