Ubuntu20 ROS noetic 自带的OpenCV版本为4.2.0，与Vins-Mono的OpenCV版本相比，接口有一些变化。
这里按照对应的Opencv4接口进行修改，可以编译通过，但还没有进一步测试。

具体的修改内容：

CV_AA -> cv::LINE_AA  
CV_GRAY2RGB -> cv::COLOR_GRAY2RGB  
CV_GRAY2BGR -> cv::COLOR_GRAY2BGR  
CV_BGR2GRAY -> cv::COLOR_BGR2GRAY  
CV_CALIB_CB_ADAPTIVE_THRESH -> cv::CALIB_CB_ADAPTIVE_THRESH   
CV_CALIB_CB_NORMALIZE_IMAGE -> cv::CALIB_CB_NORMALIZE_IMAGE  
CV_CALIB_CB_FILTER_QUADS -> cv::CALIB_CB_FILTER_QUADS  
CV_CALIB_CB_FAST_CHECK -> cv::CALIB_CB_FAST_CHECK  
CV_THRESH_BINARY -> cv::THRESH_BINARY  
CV_SHAPE_CROSS -> cv::MORPH_ELLIPSE  
CV_SHAPE_RECT -> cv::MORPH_RECT  
CV_TERMCRIT_EPS -> cv::TermCriteria::EPS  
CV_TERMCRIT_ITER -> cv::TermCriteria::MAX_ITER  
CV_RETR_CCOMP -> cv::RETR_CCOMP  
CV_CHAIN_APPROX_SIMPLE -> cv::CHAIN_APPROX_SIMPLE  
CV_CALIB_CB_FILTER_QUADS -> cv::CALIB_CB_FILTER_QUADS  
CV_THRESH_BINARY_INV -> cv::THRESH_BINARY_INV  
CV_FONT_HERSHEY_SIMPLEX -> cv::FONT_HERSHEY_SIMPLEX  