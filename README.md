Manifests for building Android for FPT mobiles
--------------

1. Installing repo tool
<pre>
  $ mkdir ~/bin
  $ PATH=~/bin:$PATH
  $ curl https://dl-ssl.google.com/dl/googlesource/git-repo/repo > ~/bin/repo
  $ chmod a+x ~/bin/repo
</pre>
2. Initialize & sync source tree
<pre>
  $ repo init -u git://github.com/manhthiep/android_fpt_mobile_manifest.git -b [branch] -m [manifest]
  $ repo sync
</pre>
3. Building
<pre>
  $ . build/envsetup.sh
  $ lunch
  $ {choose target}
  $ make -j4
</pre>
