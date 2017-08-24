VelodyneCapture
===============

VelodyneCapture is the general capture class to retrieve the laser data from Velodyne sensors using Boost.Asio and PCAP.  
VelodyneCapture will be able to retrieve lasers infomation about azimuth, vertical and distance that capture at one rotation.  
This class supports direct capture form Velodyne sensors, or capture from PCAP files.  
( This class only supports VLP-16 and HDL-32E sensor, and not supports Dual Return mode. )  


Environment
-----------
If direct capture from sensors, VelodyneCapture are requires Boost.Asio and its dependent libraries ( Boost.System, Boost.Date_Time, Boost.Regex ).  
Please define <code>HAVE_BOOST</code> in preprocessor.  
* Boost.Asio  

If capture from PCAP files, VelodyneCapture are requires PCAP.  
Please define <code>HAVE_PCAP</code> in preprocessor.  
* libpcap ( or WinPCAP )  


Sample
------
This repository has two sample programs.  
* simple  
  This sample program is displayed data on standard output.  
  This sample program depends on dependent libraries ( Boost.Asio or libpcap ( or WinPCAP ) ) of VelodyneCapture class.  

* viewer  
  This sample program is displayed data on point cloud.  
  This sample program depends on OpenCV Viz module in addition to dependent libraries ( Boost.Asio or libpcap ( or WinPCAP ) ) of VelodyneCapture class.  

License
-------
Copyright &copy; 2017 Tsukasa SUGIURA  
Distributed under the [MIT License](http://www.opensource.org/licenses/mit-license.php "MIT License | Open Source Initiative").  


Contact
-------
* Tsukasa Sugiura
    * <t.sugiura0204@gmail.com>
    * <https://twitter.com/UnaNancyOwen>
    * <http://UnaNancyOwen.com>