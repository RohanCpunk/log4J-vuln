####JDK INSTALLATION#########

steps:
1. Download jdk8 file from oracle we site "http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html"
2. Go to jvm directroy - /usr/lib/jvm
3. Extract jdk compressed archive file 
4. Add to environment variables

in the opened file add the following bin folders to the existing PATH variable Depending on your JDK version, the path can be diffrent 

CLI Command 
Now open 
>>nano /usr/lib/jvm
Add this to the env - :/usr/lib/jvm/jdk1.8.0_181/bin:/usr/lib/jvm/jdk1.8.0_181/db/bin:/usr/lib/jvm/jdk1.8.0_181/jre/bin

Add the following environment variables at the end of the file 
>> J2SDKDIR="/usr/lib/jvm/jdk1.8.0_181"
>> J2REDIR="/usr/lib/jvm/jdk1.8.0_181/jre"
>> JAVA_HOME="/usr/lib/jvm/jdk1.8.0_181"
>> DERBY_HOME="/usr/lib/jvm/jdk1.8.0_181/db"

5. Enter the following commands to inform the system about the java loaction Depending on your JDK version 

>> sudo update-alternatives --install "/usr/bin/java" "java" "/usr/lib/jvm/jdk1.8.0_181/bin/java" 0
>> sudo update-alternatives --install "/usr/bin/javac" "javac" "/usr/lib/jvm/jdk1.8.0_181/bin/javac" 0
>> sudo update-alternatives --set java /usr/lib/jvm/jdk1.8.0_181/bin/java
>> sudo update-alternatives --set javac /usr/lib/jvm/jdk1.8.0_181/bin/javac

-----------------------

Now for Alternative update or to use older version
>> update-alternative --config java

[Note : Then select the 1 or 2 as per the option]
