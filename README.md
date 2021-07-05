# shifterTest

As per https://user.cscs.ch/tools/containers/shifter/advanced_shifter/ :  
$ module load shifter-ng  
(after which any shifter commands return "shifter: error while loading shared libraries: libnettle.so.4: cannot open shared object file: No such file or directory")

OR

As per https://user.cscs.ch/tools/containers/shifter/legacy_shifter/ :  
$ module load shifter  
$ shifterimg pull afilipcic/hello-python:1.0  
(which apparently should work after having uploaded the image to dockerhub, instead returns "ERROR: failed to contact the image gateway.", same with any other image I've tried)  
$ shifter --image=docker:ubuntu/15.04  
(as the example shows in "shifter -h" also comes up with the same error)
