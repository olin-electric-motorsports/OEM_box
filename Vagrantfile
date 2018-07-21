# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "oem-box"
  config.vm.box_url = "file://~/vagrant_boxes/oem-box.json"
  config.vm.provider "virtualbox" do |vb|
    vb.customize ["modifyvm", :id, "--usb", "on"]
    vb.customize ['usbfilter', 'add', '0', '--target', :id, '--name', 'usbtiny', '--vendorid', '0x1781', '--productid', '0x0c9f']
  end

end
