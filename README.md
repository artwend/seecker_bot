# seecker_bot

> **Disclaimer:** This project is for educational purposes only.

A small OpenCV-based image processing demo (C++20). It loads an image, isolates green regions via an HSV color mask, detects circles with the Hough transform, and visualizes intermediate steps (mask, blurred image, and detected circles).

## Build

Requires CMake ≥ 3.17, a C++20 compiler, and OpenCV (plus `PThreads_windows` via vcpkg or similar).

```bash
cmake -B build
cmake --build build
```

## Run

Place the input image (`Screenshot_2021-02-25_15_17_39_120993.jpg`) next to the executable's parent directory (path is hardcoded in `main.cpp`), then run the built `seecker_bot` binary. Several windows will display the processing stages.

## License

MIT — see [LICENSE](LICENSE).

