sof-glk-es8336-ssp0.tplg# essx8336

Kernel with support for the essx8336 codec.
Tested on ubuntu, astra linux, alt linux.

# install deb on Ubuntu:
Link to download:
https://drive.google.com/drive/folders/1GJiZXnPsrxm78CJIA8dQC1UdtuDn77j0?usp=sharing

Just install the packages *.deb

Install depends:

$ apt-get install firmware-linux firmware-alsa-sof

reboot and copy:

$ cp sof-cnl.ri /lib/firmware/intel/sof/

$ cp sof-cnl.ldc /lib/firmware/intel/sof/

$ cp sof-glk-es8336-ssp0.tplg /lib/firmware/intel/sof-tplg/


# install other:
Installation into "rpm" distributions can be done by unpacking "deb" into directories.

Then:

$ make-initrd -k 5.12.6-cnl

$ update-grub

$ reboot

$ cp sof-cnl.ri /lib/firmware/intel/sof/

$ cp sof-cnl.ldc /lib/firmware/intel/sof/

$ cp sof-glk-es8336-ssp0.tplg /lib/firmware/intel/sof-tplg/
