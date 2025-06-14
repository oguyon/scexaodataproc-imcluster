# Image clustering

Generate random images to a stream:

$ ./milk-mkstream-rnd imrnd 4 4

Will run at 1000 Hz


Write 10 FITS cubes:

$ mkdir -p data

$ milk-streamFITSlog -D "$(pwd)/data" -z 10000 imrnd pstart
$ milk-streamFITSlog -c 100 imrnd on


