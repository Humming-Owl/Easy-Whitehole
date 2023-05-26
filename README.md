# Easy-Whitehole

Repository containing the usual and latest **Whitehole** versions used for **SMG1/2 modding** in a prepared form so you can get them working right away (**Win32/64 only for now**).

**All credit goes to the creators/mantainers/developers of these Whitehole versions**. I just packed them into a nice **7Z compressed file** so you can use the programs without having to set up **Java** (*Epik Java*). Also thanks to the **Adoptium** and **Liberica JDK Download Center** for the binary releases of **JRE 8 and 17** which are used in each compressed package shared.

**Adoptium** --> https://adoptium.net/download/

**Liberica JDK Download Center** --> https://bell-sw.com/pages/downloads/

# Usage

**Windows users:** 

- Use **7zip** to extract the contents of the **7Z files** shared --> https://7-zip.org/download.html
- Inside each **Whitehole folder** there is a `Whitehole-[Version].bat` file, double click on it and it should open right away!
- There is also an `UpdateObjectDatabase.bat` file on some **Whiteholes** (**v1.6** and **v1.7** specifically), double click on it to update the **Object Database**.

# IMPORTANT NOTES

- For absolute beginners **Whitehole Despag** is the one recommeded. When you get more familiarized with SMG modding you can test the other editors.
- **Whitehole Despag** will update the Object Database automatically each time you run the program (don't worry about updating it manually).
- **Whitehole for SMG1** is only used for its Scenario editor that works with SMG1.
- **Whitehole Despag** does not render gravity areas because the gravity rendering has never been accurate on any Whitehole.
- **Newer Object Databases** do not work on **Whitehole for SMG1** (program crashes).
- **Whitehole v1.7** can't open Galaxies that have unused zones. You have to manually delete unused zones of a Galaxy. 
  
  *As a quick workaround*, open the Galaxy you can't open on **Whitehole v1.7** in **Whitehole Despag** and immediately hit **Save** (`File > Save`), then, you will be able to open said Galaxy on **Whitehole v1.7**.
  
- **Whitehole v1.7** does not render well Galaxies under **Integrated Intel Graphics** in Windows (screen is black while you don't move in the editor - I've seen this happening with a few computers).
  
  *As a workaround* (**BE CAREFULL WITH THIS - USE ONLY IF NEEDED AND IF YOU KNOW WHAT YOU ARE DOING**) you can download the **Mesa3D implementation of OpenGL** for your Windows platform from here (32 or 64 bits) --> https://fdossena.com/?p=mesa/index.frag
  
  Then rename the `opengl32.dll` located at `C:\Windows\System32` to `opengl32_original.dll` (for example) and copy the `opengl32.dll` file from the package mentioned above into `C:\Windows\System32` or in the `jre\17\Win[Architecture]\bin` folder of the Whitehole tool downloaded.
  
  *If pasted on `C:\Windows\System32`* Windows will run OpenGL in "Software Mode" (not using the GPU hardware) and **ALL** programs that rely on OpenGL on Windows will run slower because of this (including **Whitehole v1.7**).
  
  *If pasted on `jre\17\Win[Architecture]\bin`* OpenGL will be only used by **Whitehole v1.7** (in "Software Mode", slow) and other programs that rely on OpenGL won't work on the system.
  
  **To revert the changes and get your original OpenGL setup** you just need to rename the `opengl32_original.dll` mentioned above to `opengl32.dll` (**be sure to always have a copy of the original `opengl32.dll` file of your Windows installation**).

# Whitehole List (latest functional release)

- Whitehole Despag (was built with **JRE 17** - https://github.com/SunakazeKun/Whitehole-Despaghettification)
- Whitehole v1.7 (was built with **JRE 17** - https://github.com/TheSunCat/Whitehole)
- Whitehole v1.6 (was built with **JRE 8** - https://github.com/TheSunCat/Whitehole)
- Whitehole for SMG1 (was built with **JRE 8** - https://github.com/SunakazeKun/Whitehole-for-SMG1)
