# Build AlphaDroid for Xiaomi Mi 9 SE (grus)

## Prerequisites
- refer to [AOSP](https://source.android.com/docs/setup/start/requirements)

## Build
1. Initialize repo with [AlphaDroid](https://github.com/AlphaDroid-Project/manifest) source code.
    ```
    repo init -u https://github.com/alphadroid-project/manifest.git -b <branch> --git-lfs
    ```

2. Clone grus manifest
    ```
    git clone https://github.com/alphadroid-devices/grus-manifest .repo/local_manifests
    ```

3. Sync
    ```
    repo sync 
    ```

4. Cook some bacon
    ```
    . build/envsetup.sh
    lunch alpha_<device>-[<release>]-user
    make bacon
    ```

    Or the light menu (no bacon)
    ```
    . build/envsetup.sh
    brunch <device>
    ```
Enjoy! :)
