# scst-3.0.x-debian
Debian packaging for SCST

This is an unofficial repository containing Debian packaging for SCST 3.0.x.
The work was originally done by Fajar A. Nugraha &lt;ubuntu-ppa@fajar.net&gt; for
the packages that can be found in this Launchpad PPA, that serves SCST
packages for Ubuntu Precise, Trusty and Utopic:

https://launchpad.net/~scst/+archive/ubuntu/3.0.x/+packages

Since I haven't been able to find something similar for Debian Jessie or
Wheezy, I adapted Fajar's work for Debian Jessie.

The quick'n'dirty howto for this repo is this:

* check out the source code for SCST from Souceforge (Svn) or Github (Git)
* check out this repository as 'debian' in the source tree
* dpkg-buildpackage / pdebuild / ...

Get the source code here:

http://sourceforge.net/p/scst/svn/HEAD/tree/branches/3.0.x/
https://github.com/bvanassche/scst/tree/svn-3.0.x

The packaging and the resulting packages HAVE NOT BEEN THOROUGHLY TESTED.
Use them at your own risk. The contents of this repository on every
tagged commit /should/ at least produce a clean build with pbuilder.

If your build fails, you can try this before starting your build tool:

  export CFLAGS="-I`pwd`/scst/include -D_GNU_SOURCE"
