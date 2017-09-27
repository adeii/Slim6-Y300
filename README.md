slimkat_manifest - experimental build with best from CAF build to legacy-display build
================

Local Manifest to build SlimKat for the Huawei Y300, G330 & G510

Build Instructions for SlimKat Y300 (U8833), G330 (U8825) & G510 (U8951)
-----------------------------------------------------------------------------

1. Initialize repo using the SlimKat manifest (legacy display branch)
    
        repo init -u git://github.com/adeii/Slim6-Y300.git -b kklegacy

2. Then sync up the repositories
 
        repo sync --force-sync --no-tags --no-clone-bundle -f

3. Some patching needing here (to original projects) and delete all "...y300" projects 

4. Initialize the build environment

        . build/envsetup.sh
    
5. Build the ROM

        For G330:
            brunch u8825
        For Y300:
            brunch u8833
        For G510:
            brunch u8951
