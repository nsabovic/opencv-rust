* 0.28
  * dnn::BackendNode constructor as well as stitching::createStitcher and stitching::createStitcherScans are no
    longer generated for the OpenCV version where they are not available, fixing the linking issues

* 0.27.0
  * add support for `vcpkg` when building for windows, it's being used by default in the absence of
    environment variables
    
  * with `buildtime-bidngen` feature enabled the crate no longer uses bundled source files for code
    generation by default, but the ones installed with OpenCV library detected by `pkg_config`, `vcpkg` or
    environment; set `OPENCV_HEADER_DIR` environment variable to override this behavior  

* 0.26.6
  * ...