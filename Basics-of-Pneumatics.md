# Basics of Pneumatics

First, you need to understand exactly what Pneumatics is and how we use it on the bot. 

Pneumatics is the branch of physics or technology concerned with the mechanical properties of gases.

This allows for us to use compressed air to control pistons for many functions such as changing gears in the drivetrain, to creating a flapper that goes back and forth.

![](https://sites.google.com/a/mypisd.net/nicholas-wharton/home/Finished-PDiagram.PNG)

The diagram above shows a basic pneumatic system which starts with the PCM.

The PCM is a Pneumatics Control Module. The PCM is what gives you control over the compressor and the solenoids that you will be using. The PCM is integrated into WPILib so you can easily access it in your code. The PCM is also a CAN based system so you just slap it on the CAN Bus.                      

![](http://www.fightingpi.org/Resources/Controls/Beta/2015_Pictures/pcm.jpg)

The compressor is a device that takes power and converts it into pressurized air. The Compressor plugs into the compressor out labeled spot on the PCM.

![](https://cdn3.volusion.com/vyfsn.knvgw/v/vspfiles/photos/am-2005-2.jpg?1442240393)  

The pressure relief valve isn't on the diagram but it is connected to the compressor via hard fittings, and it is basically a pressure regulator. It is in the FRC rules that you have to have it set to 60 psi.
![](https://cdn3.volusion.com/vyfsn.knvgw/v/vspfiles/photos/am-2002-2.jpg?1442240393)

The pressure switch is used to determine the compressor's state. this information is what is used by the PCM to handle turning on and off the compressor. The pressure switch plugs into the spot on the PCM that is labeled PRESSURE SW.

![](https://cdn3.volusion.com/vyfsn.knvgw/v/vspfiles/photos/am-2006-2.jpg?1442240393)

The tank or the accumulator is used to hold compressed air that comes out of the compressor.

![](http://www.myfishtank.net/wordpress/wp-content/uploads/fishtank-tshirt.gif)

The primary pressure regulator also is known as the relieving regulator. This means that it limits the downstream system pressure and is used to relieve excess pressure that could have been gained in the downstream part of the system. Also, this regulator usually has a gauge so you are able to see the amount of pressure.                                                                                         

![](https://d25g25bk48as5o.cloudfront.net/images/243x/R07.jpg)

The solenoid is a valve that opens and closes to release air. The solenoid is connected and controlled by the PCM and the PCM WPILib functions. You connect the solenoid into one of the solenoid ports. With the PCM that we use you can connect up to 8 different solenoids to it.

![](http://www.team358.org/files/pneumatic/Festo24v.jpg)

One other thing about solenoids is there are singles and there are doubles. The picture above is a double solenoid which means that you have one input and two output valves. With a double solenoid, you have to use two of the solenoid spots on the PCM to plug it in.

The piston is a device that uses compressed gas to produce a force in a reciprocating linear motion. Taking the air that is let out by the solenoid you can move the piston. If you have a double solenoid you are able to move the piston out and back in, but with a single piston, you are only able to let the piston out.

![](http://www.airtec.de/tl_files/products/Pneumatikprogramm/Pneumatikzylinder%20mit%20Kolbenstange/images/HM-25-080.jpg)

That really is everything that you will need for the basics of pneumatics if you would like to know more go to the FIRST Pneumatics Manual [here](http://kellrobotics.org/files/pdf/2015-frc-pneumatics-manual.pdf).







