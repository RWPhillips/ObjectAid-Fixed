# ObjectAid-Fixed

- [About this Project](#project)
- [Important-- Read This](#important)
- [Instructions](#instructions)
- [FAQ](#faq)
<br /><br />

<a name="project"></a>
## ABOUT THIS PROJECT:

This is the ObjectAid plugin for Eclipse, updated to work with Eclipse in 2023 with Java 17 (at least).
ObjectAid's developer was in a tragic accident, therefore ObjectAid has not been updated since. As Eclipse has been updated in recent years, ObjectAid had stopped working. I was able to find out what was wrong with ObjectAid and get it working with the latest version of Eclipse. Therefore, I'm sharing this file in hopes this can help others who are also looking for a UML solution.
<br /><br /><br />

<a name="important"></a>
## IMPORTANT-- READ THIS:

### Update July 6th, 2023: 
I've added an FAQ at the bottom of this document, that I suggest everyone read before doing the installation.

There are two version of ObjectAid I've uploaded. The ObjectAid-Fixed is the version I've used with success, but the ObjectAid with xStream 1.4.20 is the latest possible update to this file (future-proof version). Both should work, just one is tested more than the other.
Also, this isn't fool-proof. I've had installations work and others that broke. I would install this on a clean copy of Eclipse, separate from your main Eclipse installation, and it may take a few tries to install correctly-- just a warning.
<br /><br /><br />

<a name="instructions"></a>
## INSTRUCTIONS FOR WINDOWS / MAC OS:

Before you do anything, add the following lines to your eclipse.ini and save it.
(at the bottom, the first one may already be there)
```
--add-opens=java.base/java.lang=ALL-UNNAMED  
--add-opens=java.base/java.util=ALL-UNNAMED  
--add-opens=java.base/java.text=ALL-UNNAMED  
--add-opens=java.desktop/java.awt.font=ALL-UNNAMED
```

1. Open Eclipse
2. Go to Help -> Install New Software

> NOTE: If you have a broken version of ObjectAid already installed, you'll need to remove it by clicking "already installed?" and uninstalling anything labeled with ObjectAid, before continuing.

3. Click Add..
4. Select Archive and pick one of the files I've uploaded
5. Set the name to ObjectAid
6. Next / Accept / Trust anything that comes up
7. Restart Eclipse and ObjectAid should be fully functional now

### Feel free to leave feedback, ask questions, or share your experiences!
<br />

<a name="faq"></a>
## FAQ:

### I See Errors and I Can Open The ObjectAid Window, But The Button Doesn't Work!

Hopefully you followed my advice and installed this on a second, clean version of Eclipse, because this is what happens if the installation messes up BUT not all is lost! 

Although broken, you can still generate UMLs, you just need a blank .ucls file. I'm not sure why this happens, but the only thing broken in this install is that you cannot generate the .ucls files-- so you CAN generate UMLs, you just can't create the file that holds them. That's why I have now generated and provided the blank.ucls above for you to rename / use as many times as you need. 

Download the blank.ucls file, put it in your folder with your project, then drag the files over into the UML. You will recieve errors (Eclipse will seem really pissed about it) but you can ignore the errors / click OK and it will generate the UML just fine. You can even right-click and save it as an image!
