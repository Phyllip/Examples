cmake_minimum_required(VERSION 2.6)

PROJECT(ReadImage)

FIND_PACKAGE(OpenCV REQUIRED )
INCLUDE_DIRECTORIES( ${OPENCV_INCLUDE_DIR} )

ADD_EXECUTABLE(ReadImage ReadImage.cxx)
TARGET_LINK_LIBRARIES(ReadImage opencv_core opencv_highgui
opencv_flann opencv_imgproc opencv_highgui opencv_ml opencv_video opencv_objdetect
          opencv_features2d opencv_calib3d opencv_legacy opencv_contrib
)