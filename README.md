Slim6 manifest for Huawei msm7x27a devices

All credits goes to chil360. This is just forked local manifest for Slim6 rom.

Build Instructions

Initialize repo using the Slim6 manifest (CAF branch)

 repo init -u git://github.com/SlimRoms/platform_manifest.git -b mm6.0
Add my local manifest

 mkdir .repo/local_manifests
 Copy slim6_huawei.xml to .repo/local_manifests
Then sync up the repositories

 repo sync
Initialize the build environment

 source build/envsetup.sh
If everything is OK, build the ROM

 For Y300:
     brunch u8833
 For G510:
     brunch u8951
 For G330:
     brunch u8825
Disclaimer - I'm not responding if this can not compile, build, etc. etc. or distroy your Huawei or bootloop or etc. etc.
