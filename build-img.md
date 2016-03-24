- Use EXTRA_IMAGE_FEATURES to generate debug symbol  

  ```
git clone https://git.openswitch.net/openswitch/ops-build 
cd ops-build
echo 'EXTRA_IMAGE_FEATURES="dbg-pkgs"' >> build/conf/local.conf
make configure genericx86-64
make
  ```
