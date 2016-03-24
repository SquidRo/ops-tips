1. Install ops-vsi and mininet
  ```
sudo apt-get install python-pip
sudo pip install pytest
cd ~
git clone git://git.openswitch.net/openswitch/ops-vsi
cd ops-vsi
sudo ./setup.py install

git clone git://github.com/mininet/mininet
cd mininet
git checkout -b 2.2.1 2.2.1
util/install.sh
  ```

2. Build an openswitch image

3. Import a docker image for mininet
  ```
  make export_docker_image openswitch/genericx86-64
  ```
