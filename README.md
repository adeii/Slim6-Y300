slim6_manifest
================

TESTING Local Manifest to TEST build Slim6 for the Huawei Y300/G510/G330
Assume: There is small diff between SlimLP-Y300 and CM13-Y300 (except kernel)!
        How about to use slimlp_huawei.xml to build Slim6-Y300 ?!

Build Instructions
-----------------------------------------------------------------------------

1. Initialize repo using the Slim6 manifest (CAF branch)
    
        repo init -u git://github.com/SlimRoms/platform_manifest.git -b mm6.0

2. Add my local manifest

        mkdir .repo/local_manifests
        Copy slim6_huawei.xml to .repo/local_manifests

3. Then sync up the repositories
 
        repo sync

4. Initialize the build environment

        source build/envsetup.sh
    
5. If everything is OK, build the ROM

        For Y300:
            brunch u8833
        For G510:
            brunch u8951
        For G330:
            brunch u8825
6. Disclaimer - I'm not responding if this can not compile, build, etc. etc. or distroy your Huawei or bootloop or etc. etc.
