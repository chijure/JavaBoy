
                                 JavaBoy v0.9
                     The portable Gameboy emulator for Java
               http://www.millstone.demon.co.uk/download/javaboy

                                     FAQ

This frequently aked questions page answers everything you'd never wanted
to know about JavaBoy.


Q: What does JavaBoy actually do?

A: JavaBoy is an emulator. An emulator is a piece of software which performs
tasks usually done by hardware. In this case, the emulator allows you to
play games written for the Gameboy or Gameboy Color on the PC (or any other
platform)

Q: What do I need to run JavaBoy?

A: JavaBoy requires at least a Pentium II/266 processor to run, and a
Pentium II/600 is reccommended for Colour Gameboy games. You will also need
to have a Java Virtual Machine installed. You can download this from Sun or
IBM, although the IBM one will provide much better performance.

Q: How do I start JavaBoy?

A: To run JavaBoy, once you have installed your Virtual Machine, simply
unzip the ZIP file into any directory, start a DOS prompt, and type

        java JavaBoy

when you are in the relevant directory, remebering to ensure the
capitalization is correct. If this doesn't work, make sure that the Java
Virtual Machine is on your path, and that you are in the correct directory.

Q: Then what do I do?

A: You need a ROM for the game you want to play. This is an image of a
Gameboy cartridge. There are several freeware ROMS available on this site.
ROMs for commercial games are under copyright. You might be able to find
them on the net somewhere, but please don't ask me for them. It's only
legal to own a ROM image if you also own the original game cartridge.

Once you've got your ROM, click 'File', 'Open ROM...', and then select
your ROM file. Then click 'File', 'Emulate'. The game should run.

Q: What are the keys? 

A: Use the cursor arrows for the D-pad. 'Z' for the A button, 'X' for the
B button, Return for the start button, and backspace for the select
button. You can change these keys using the 'Define Controls..' option on
the file menu.

Q: Why is everything so slow? 

A: Java programs are interpreted, so the speed is less than ideal. To
speed up the emulator, you can use a smaller window from the 'View' menu.
You can also force it to display less frames. The action is more jerky,
but the game will run faster. To adjust frame skip, press F1 and F2 on
your keyboard.

Q: How do I use JavaBoy as an applet on a web page? 

A: First, create an HTML file with the following tag: 

<APPLET CODE="JavaBoy.class" WIDTH=160 HEIGHT=144>
<PARAM NAME="ROMIMAGE" VALUE="*Enter name of ROM image here*">
<PARAM NAME="SOUND" VALUE="ON">
</APPLET> 

Then, place the HTML file, the ROM image, and all the emulator files 
(*.class), in the same directory, and open the HTML file
in a browser. You should be able to play the game in the browser, after
clicking on the applet window to give it the keyboard focus. A reduced
feature set is available when JavaBoy is running as an applet. Only a
1x view is supported, and black and white games can only be played with
the standard colours. More features may be supported in the next version.
One advantage to this mode is that the user needn't install a Java
runtime environment, as the necessary libraries are supplied with your
web browser.

Q: Can JavaBoy load compressed ROM images? 

A: Yes, ROMs can be loaded in ZIP/JAR or GZip format. In the application
version, just select the name of the Zip file when you choose File/Open. 
For the applet version, use the name of the Zip file in the "ROMIMAGE" 
parameter to the applet. For ZIP/JAR files, the first .GB or .GBC file 
in the Zip will be used. GZip files cannot be Tarred, or they won't work. 

Q: Can I use JavaBoy on my web page? 

A: That depends. If you page is non-commercial, then you can use JavaBoy 
all you want. If your page is commercial, then you ned to email me to 
discuss licencing conditions. 

Q: How do I use the networking feature? 

Networking allows you to play certain games against other players on a
LAN or the Internet. This feature is very much in it's infancy, and it
has only been shown to work with three games, (Tetris, Dr Mario, and
Dynablaster) so you may not have much luck with any others.

To use the feature, you need two machines on the same TCP/IP network.
Run JavaBoy on both machines, and load the same ROM. On one machine,
choose 'Allow connections' from the 'Network' menu. On the other
machine, choose 'Connect to client' from the 'Network' menu. Enter
the IP address of the other machine in the box and click ok. You
will be notified when the connection is made. Then start the two player
game as if you were running on two linked Gameboys. Be patient, as games
are often punctuated by long pauses as the machines communicate.

Q: What do the colour schemes do? 

A: The colour schemes can be found at the bottom of the 'View' menu. These
alow black & white games to be given a kind of 'false colour'. Select one
of the options to see what it's like. The 'LCD Shades' option tries to
reproduce the yellow shades on the original Gameboy. This will have no effect
on colour games.

Q: Why won't my game work? 

A: The compatibility of the emulator is not 100%, and there are several known
games which don't work, or display major faults. If you find a game which is
not listed on the compatibility page which doesn't work, email me and I may
fix it in a later version. No promises though, as these things are
notoriously hard to track now.

Q: How do I compile JavaBoy? 

A: To compile JavaBoy, you will need the source archive, which can be found
on the downloads page. You will also need a compiler which supports Java 1.2
(Java2 Revision 1.2). You can find this on Sun's site, amoung others. Once
you have this, simply type:

        javac -O JavaBoy.java

The necessary .class files will then be created.

Q: What's the debugger for? 

A: If you have to ask, you don't need it. 

Q: What's the meaning of life, the universe, and everything? 

A: That's easy, it's 42. 

