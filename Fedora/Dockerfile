FROM fedora:latest
MAINTAINER Philipp Moeller <bootsarehax@gmail.com>

RUN yum -y update; yum clean all
RUN yum -y install make cmake gcc-c++ tar \
                   glibc-devel.x86_64 libstdc++-devel.x86_64 \
                   gmp-devel.x86_64 mpfr-devel.x86_64 \
                   boost-devel.x86_64 \
                   qt3-devel.x86_64 qt-devel.x86_64 \
                   libQGLViewer-devel.x86_64 \
                   /usr/lib64/libX11.so /usr/lib64/libSM.so \
                   /usr/lib64/libpng.so /usr/lib64/libICE.so \
                   /usr/lib64/libGL.so /usr/lib64/libGLU.so \
                   /usr/lib64/libXi.so /usr/lib64/libXrender.so \
                   /usr/lib64/libXrandr.so /usr/lib64/libXcursor.so \
                   /usr/lib64/libXinerama.so \
                   /usr/lib64/libXfixes.so /usr/lib64/libXext.so \
                   /usr/lib64/libXdamage.so /usr/lib64/libXft.so \
                   /usr/lib64/libXt.so /usr/lib64/libXau.so \
                   /usr/lib64/libXxf86vm.so /usr/lib64/libjpeg.so \
                   /usr/lib64/libxcb.so /usr/lib64/libdrm.so \
                   /usr/lib64/libfreetype.so /usr/lib64/libfontconfig.so \
                   zlib-devel.x86_64
RUN yum clean all

ENV QTDIR=/usr/lib/qt-3.3/
ENV QTINC=/usr/lib/qt-3.3/include/
ENV QTLIB=/usr/lib/qt-3.3/lib/

ENV CGAL_TEST_PLATFORM="Fedora"
ENV CGAL_CMAKE_FLAGS=""