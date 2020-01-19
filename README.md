# podman Setup for Raspbery Pi
Download, compile and install named-releases of Podman / Buildah and Skopeo for a Raspberry Pi.  

## Gotcha
   * Pi's do not have enough memory to link buildah or podman - Swap space must be enabled.
      * I've left in brute-force automation to enable/disable swap for the build. If this proves troublesome, a command line switch can be provided to  


## FIXME
   * (Randomly) Go reports not enough memory to link - manual compilation is fine. Perhaps an ansible'ism
   * Due to the above - I'm not cleaning up automatically. A special tag podman_build_cleanup is required to delete tmp data.
   * For the same reasons, I'm not removing the development libraries.
