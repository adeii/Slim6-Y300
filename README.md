slim6_manifest
================

All credits goes to chil360. This is just forked local manifest for TESTING Slim6 rom for Huawei Y300.

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
