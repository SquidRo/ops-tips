- Build openswitch image for mininet

(Use EXTRA_IMAGE_FEATURES to generate debug symbol.
Refer to http://www.openswitch.net/documents/dev/how-to-debug
Refer to http://www.openswitch.net/documents/dev/step-by-step-guide 
for complete steps to build an image)

```
git clone https://git.openswitch.net/openswitch/ops-build 
cd ops-build
echo 'EXTRA_IMAGE_FEATURES="dbg-pkgs"' >> build/conf/local.conf
make configure genericx86-64
make
```
