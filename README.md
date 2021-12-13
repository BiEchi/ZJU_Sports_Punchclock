# ZJU_Sports_Punchclock
Wanna punch sports clock automatically? Try this! This tutorial is for those who have both Mac and iPhone.

[TOC]

## Install Xcode of the latest version

Because the development is based on iOS system, we use Xcode to construct the project and simulate the whole process. Note that if you want to do this on a real phone, you need to connect your iPhone to your Mac.

## Get your location of latitude and longitude

Open [Gaode API](https://lbs.amap.com/tools/picker) and get your intended location. Note that this location (GCJ02) is not exact because of restrictions in China. Thus, the real location should be obtained by a mathematical algorithm.

## Use the shift algorithm from GCJ02 to WGS84

Modify the main function in the python script `./coordTransform_utils.py` and run `python2 ./coordTransform_utils.py` to get the real location.

## Construct the Program

Open Xcode, and build a new program. Create a new GPX file.

![image-20211213205015924](http://jacklovespictures.oss-cn-beijing.aliyuncs.com/2021-12-13-125016.png)

![image-20211213205033710](http://jacklovespictures.oss-cn-beijing.aliyuncs.com/2021-12-13-125034.png)

Copy and paste the exact location (latitude and longtitude) into the file.

![image-20211213205236863](http://jacklovespictures.oss-cn-beijing.aliyuncs.com/2021-12-13-125237.png)

## Run the program on your phone

Edit the scheme of the program to real phone and click “run”.

![image-20211213205156975](http://jacklovespictures.oss-cn-beijing.aliyuncs.com/2021-12-13-125157.png)

Then stop running and run the program for several times, and then the location is successfully shifting from your place now to another place!
