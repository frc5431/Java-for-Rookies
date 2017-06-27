# Installing Java for Robots

First, we need to install the JDK onto our computer so we can actually write Java code! The RoboRIO has JRE version 8, meaning we need to use JDK version 8. Pretty simple!

We have to use Windows for Robot development because its the only OS that WPILib supports.

Go to the [Java website](http://www.oracle.com/technetwork/java/javase/downloads/index.html) and find where it says to download the Java Platform \(JDK\)

![](/assets/jdk-download)

Accept the license agreement and scroll down until you find Windows. If you are on a x64 bit computer, download the x64 bit version of the JDK. Otherwise, download the x32 bit version.

![](https://s3.amazonaws.com/screensteps_live/image_assets/assets/000/289/046/original/1404865f-a77a-4a8a-b605-66c8e1398c3f.png?1483509863)

Run the installer and complete it. Now you can program in Java 8!

To help use write Java code, we will use an IDE \(Integrated Developer Environment.\) An IDE is a handy program that does a lot of the hard work for you, like configuring the JDK to compile your program. All you need to do is write your Java code and hit the big green run button and your IDE will do what it needs to do.

The IDE we will be using is called Eclipse. It is probably the most popular IDE for Java out there.

Eclipse can be downloaded from their website [http://www.eclipse.org/](http://www.eclipse.org/). Just click the big download button:![](https://wpilib.screenstepslive.com/s/4485/m/13809/l/599681-installing-eclipse-c-java/show_image?image_id=289058)You should reach a new page. Click the "Download Packages" link.![](/assets/eclipse-download-packages)Find where it says Eclipse IDE for Java developers and download either the x64 or x32 bit version. **It must match the version of the JDK you downloaded.**![](/installing-java/eclipse-installer)Extract the downloaded file.

![](https://s3.amazonaws.com/screensteps_live/image_assets/assets/000/289/040/original/cae7cd79-be96-410c-a139-718ef4e0348d.png?1483509857)

Then move the extracted files to Program Files

![](https://s3.amazonaws.com/screensteps_live/image_assets/assets/000/289/044/original/289f5a53-a538-4d53-aabb-f591337961e4.png?1483509861)

Now you can just run eclipse.exe and you should see something like this:

![](https://s3.amazonaws.com/screensteps_live/image_assets/assets/000/289/062/original/bc5d22a2-dc6c-43aa-85b9-791a93ae9a96.png?1483509883)

Check the "Use this as the default and do not ask again" box and click OK. This is the directory where your projects will be stored in.

## FRC Plugins

Now you also need WPILib to allow you to interact with the RoboRIO. 

Go to Help &gt; Install New Software. Then click the Add... button to add the FRC site. Call the Repository FRC plugins and the location is http://first.wpi.edu/FRC/roborio/release/eclipse/![](https://s3.amazonaws.com/screensteps_live/image_assets/assets/000/289/021/medium/7255971c-a1a7-4f32-91d9-7b868f5604c8.png?1483509837)Now check the box that says "Robot Java Development" and install it.

![](https://s3.amazonaws.com/screensteps_live/image_assets/assets/000/289/033/medium/98cc09fa-fca6-4426-84c1-e82655863389.png?1483509850)

That is it! Everything should be set up. If you need more detailed instructions or need to start over, look at the official tutorial to do this step: [https://wpilib.screenstepslive.com/s/4485/m/13809/l/599681-installing-eclipse-c-java](https://wpilib.screenstepslive.com/s/4485/m/13809/l/599681-installing-eclipse-c-java)

