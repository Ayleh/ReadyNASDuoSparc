# Install

1. Copy this folder (gcc-7.1) to /c/opt/
2. `cd /opt/`
2. Create a symlink from /opt/gcc-7.1 -> /c/opt/gcc-7.1 with `ln -s /c/opt/gcc-7.1/ gcc-7.1`
3. ` tar xvfz /opt/gcc-7.1/libexec/gcc/sparc-unknown-linux-gnu/7.1.0/cc1plus.tar.gz` (this file was compressed dueo file size limit on github)
4. Remove rm `/opt/gcc-7.1/libexec/gcc/sparc-unknown-linux-gnu/7.1.0/cc1plus.tar.gz`
5. Add folder to LD_LIBRARY with `export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/opt/gcc-7.1/lib/`
6. `chmod +x /opt/gcc-7.1/bin/*`
7. Set CC and CXX param when compiling stuff e.g. ./configure CC=/opt/gcc-7.1/bin/gcc CXX=/opt/gcc-7.1/bin/g++

# Requirements:

When installing the packages and you encounter an error while processing the deb packages try for example ` dpkg -i --force-overwrite ../mpc-1.0.3_1.0.3-1_sparc.deb     `

1. libisl
2. mpc
3. gmp
4. mpfr
 autoconf-2.69_1.5.3-1_sparc.deb 
 automake-1.15.1_1.15.1-1_sparc.deb 
 bison-3.0.4_3.0.4-1_sparc.deb 
 flex-2.6.4_1.5.3-1_sparc.deb 
 gettext-0.19.8.1_0.19.8.1-1_sparc.deb 
 libtool-2.4.6_2.4.6-1_sparc.deb 
 m4-1.4.18_1.4.18-1_sparc.deb 
 make-4.2.1_1.5.3-1_sparc.deb 
