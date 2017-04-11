# Description
Running this simple maven app you can create an small Update Site containing one runtime version already present in the public update site with the intention of sharing a single runtime version for Studio to soneone that can not access to Public Update Site through Studio. 

The current runtimes Update Site size is around the 5 GB which is too heavy to be sent and this should generate a private update site of around 260 MBs.

# Use 

* Clone this repo
* Open the Pom.xml and set the property mule.runtime.version to the version of the runtime you would like to create the Private Update Site. 
* Go to the commanline and run: mvn package 

In the Trarget you will have the uncompressed Update Site that you can test under the folder *repository* and the ziped Update Site to be sent under the file update-site-${runtime-version}.zip 
