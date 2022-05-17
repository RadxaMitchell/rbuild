```
.github             GitHub workflow related files.
.rootfs             Untracked folder containing rootfs generated by the last build.
                    Can be used to speed up image generation the next time.

common              rbuild scripts
    .packages       Untracked folder for soft linking local packages
    overlays        Various overlays for directly applying onto rootfs
    add_repo.yaml   Adding custom apt repo in rootfs
    clean.yaml      Common clean up script
    hack_install_deb.yaml
                    HACK for installing local package.
                    Only for debug use. Repo should not contain prebuild deb packages.
    hw-info.conf    Stores SoC's vendor and each vendor's preferred partition table type.
    image.yaml      Core script for deploying a rootfs to disk image.
                    Also install device specific kernel and firmware.
    rootfs.sh       Prepare the system for first boot.
    rootfs.yaml     Core script for generating a device-agnostic rootfs.
    sdboot.sh       Additional script for setting systemd-boot.

.gitignore          gitignore file
configs             Board specific configs.
docs                Documentation.
action.yaml         GitHub custom action file. Allow this repo to be used in GitHub Workflow.
rbuild              Main script.
README.md           Generic readme.
```