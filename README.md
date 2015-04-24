# tess4jtest
An example Java project for using tess4j, a Java wrapper for tesseract_ocr.

To build the project by following the steps

1. ldd libtesseract.so
2. wget http://launchpadlibrarian.net/149178897/libtiff4_3.9.7-2ubuntu1_amd64.deb
3. dpkg -i libtiff4_3.9.7-2ubuntu1_amd64.deb
4. sudo apt-get install libjpeg62
5. export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:`pwd`
6. export TESSDATA_PREFIX=`pwd`
7. java -cp .:lib/ghost4j-0.3.1.jar:lib/jai_imageio.jar:lib/jna.jar:lib/junit-4.10.jar:lib/nblibraries.properties:lib/pdfpagecount.ps:lib/tess4j.jar:bin -Djava.library.path=/home/l1z2g9/Applications/tess4jtest/ -Djna.platform.library.path=/home/l1z2g9/Applications/tess4jtest/ TesseractExample
8. javac -cp .:lib/ghost4j-0.3.1.jar:lib/jai_imageio.jar:lib/jna.jar:lib/junit-4.10.jar:lib/nblibraries.properties:lib/pdfpagecount.ps:lib/tess4j.jar src/TesseractExample.java -d bin/
