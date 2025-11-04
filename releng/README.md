Build steps:
1. clone repo
2. make a backup of ``releng/airootfs``
3. run ``git clone https://github.com/bootc-dev/bootc.git /tmp/bootc && \
    cd /tmp/bootc && \
    make bin install-all install-initramfs-dracut DESTDIR=/path/to/netC-archiso/releng/airootfs``
4. cd to ``/path/to/netC-archiso``
5. run ``sudo mkarchiso -v -w /path/to/netC-archiso/output -o /path/to/netC-archiso/output releng/``
