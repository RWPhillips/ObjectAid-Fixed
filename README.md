# ObjectAid-Fixed

ABOUT THIS PROJECT:

This is the ObjectAid plugin for Eclipse, updated to work with Eclipse in 2023 with Java 17 (at least).
ObjectAid's developer was in a tragic accident, therefore ObjectAid has not been updated since. As Eclipse has been updated in recent years, ObjectAid had stopped working. I was able to find out what was wrong with ObjectAid and get it working with the latest version of Eclipse. Therefore, I'm sharing this file in hopes this can help others who are also looking for a UML solution.

IMPORTANT-- READ THIS:

There are two version of ObjectAid I've uploaded. The ObjectAid-Fixed is the version I've used with success, but the ObjectAid with xStream 1.4.20 is the latest possible update to this file (future-proof version). Both should work, just one is tested more than the other.
Also, this isn't fool-proof. I've had installations work and others that broke. I would install this on a clean copy of Eclipse, separate from your main Eclipse installation, and it may take a few tries to install correctly-- just a warning.

INSTRUCTIONS:

Before you do anything, add the following lines to your eclipse.ini and save it.
(at the bottom, the first one may already be there)

--add-opens=java.base/java.lang=ALL-UNNAMED  
--add-opens=java.base/java.util=ALL-UNNAMED  
--add-opens=java.base/java.text=ALL-UNNAMED  
--add-opens=java.desktop/java.awt.font=ALL-UNNAMED

1. Open Eclipse
2. Go to Help -> Install New Software

NOTE: If you have a broken version of ObjectAid already installed, you'll need to remove it by clicking "already installed?" and uninstalling anything labeled with ObjectAid, before continuing.

3. Click Add..
4. Select Archive and pick one of the files I've uploaded
5. Set the name to ObjectAid
6. Next / Accept / Trust anything that comes up
7. Restart Eclipse and ObjectAid should be fully functional now

Feel free to leave feedback, ask questions, or share your experiences!
