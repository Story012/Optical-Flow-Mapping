# Optical-Flow-Mapping

![canny_filter.png](https://github.com/Story012/Optical-Flow-Mapping/blob/main/Flow%20mapping%20Images%20git/canny_filter.png)
1. Canny filter of edges. <br>
![dense_optical_flow_of_edges.png](https://github.com/Story012/Optical-Flow-Mapping/blob/main/Flow%20mapping%20Images%20git/dense_optical_flow_of_edges.png)
2. Dense optical flow of edges. <br>
![hough_lines.png](https://github.com/Story012/Optical-Flow-Mapping/blob/main/Flow%20mapping%20Images%20git/hough_lines.png)
3. Hough lines. <br>
![independent_hough_lines.png](https://github.com/Story012/Optical-Flow-Mapping/blob/main/Flow%20mapping%20Images%20git/independent_hough_lines.png)
4. Independently selected hough lines. <br>

# Running the scripts
To run the script sucessfully, ensure VideoCapture is set to either dev0 (a usb or built-in webcam) or a file, in which you must specify paths. 

```
git clone https://github.com/Story012/Optical-Flow-Mapping.git
mkdir build && cd build
cmake ..
make
./opt_flow
```
