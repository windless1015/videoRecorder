# videoRecorder
Record usb camera to avi file by using .net Accord library

The key problem is: 
_writer.Open(dialog.FileName, 1280, 720, 25, VideoCodec.MPEG4, 4000000);
1.the fourth parameter is framerate, if it is set by 17fps, the program will throw a exceptioin 1
2.the fifth parameter is codec type, if it is set by other type like H264, the program will throw a exceptioin 2
3.the last parameter is bitrate, if it is set by default ,the quality is low. when look up the video file information, the bitrate is 400kbps. 4000kbps is good enough.
