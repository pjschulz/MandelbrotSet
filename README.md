# MandelbrotSet
Create an ASCII PPM image of the Mandelbrot set
-Full Name: Patrick Schulz
-Project Name: "MandelbrotSet"
-Problem 3: Generating an image of the Mandelbrot set, using OpenMP
-This program was taken from https://people.sc.fsu.edu/~jburkardt/c_src/mandelbrot_openmp/mandelbrot_openmp.html
-Known Issues: 
  - At first the program did not run for me, I was receiving a seg fault at the line containing "int g[m][n]"
  - I changed the m and n values from 500 to 300 to fix this issue
-Tested on Windows 10
-used https://convertio.co/ppm-png/ to convert ppm image to png
-Expected Output:
ppm image is saved in 
C:\Users\...\CLionProjects\MandelbrotSet\cmake-build-debug\mandelbrot.ppm

C:\Users\...\CLionProjects\MandelbrotSet\cmake-build-debug\MandelbrotSet.exe
10 December 2017 10:36:04 PM

MANDELBROT_OPENMP
  C/OpenMP version

  Create an ASCII PPM image of the Mandelbrot set.

  For each point C = X + i*Y
  with X range [-2.25,1.25]
  and  Y range [-1.75,1.75]
  carry out 2000 iterations of the map
  Z(n+1) = Z(n)^2 + C.
  If the iterates stay bounded (norm less than 2)
  then C is taken to be a member of the set.

  An ASCII PPM image of the set is created using
    M = 300 pixels in the X direction and
    N = 300 pixels in the Y direction.

  Time = 0.0711838 seconds.

  Graphics data written to "mandelbrot.ppm".

MANDELBROT_OPENMP
  Normal end of execution.

10 December 2017 10:36:04 PM
