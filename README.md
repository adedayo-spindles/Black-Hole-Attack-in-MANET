If ns-3 is "not installed" in your machine:

1. Download ns-allinone-3.25.tar.bz2

2. Download Blackhole-ns-3.25.patch

3. Unzip ns-allinone-3.25.tar.bz2. You will get a folder named ns-allinone-3.25

4. Paste the downloaded Blackhole-ns3 patch in the above mentioned folder.

5. Give the following command:

patch -p1 < Blackhole-ns-3.25.patch

6. Go in ns-allinone-3.25 via terminal and give the following command to install ns-3.25

./build.py --enable-examples --enable-tests

You are done with it!

If ns-3 is "already installed" on your machine:

1. Paste the downloaded Blackhole-ns-3.25 patch in ns-allinone-3.25 directory.

2. Give the following command:

patch -p1 < Blackhole-ns-3.25.patch

3. Go in ns-allinone-3.25/ns-3.25 directory and give the following commands:

./waf

You are done with it!
---------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------

AFTER done these steps download the zipped folder from the link given below and extract the files from it:

Put both the extracted files in the following folder:

ns-allinone-3.25/ns-3.25/scratch

How to use these files for verification?

I. Go to ns-allinone-3.25/ns-3.25 via terminal and give the following command:

./waf --run scratch/blackhole
