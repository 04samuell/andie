## Introduction
> Weclome to A-Team's Amazing ANDIE Application.

ANDIE is a non destructive image editor developed entirely in java by myself and four other students for a university assignment. We started with the source code provided to us by staff and added a range of features and improvements over the course of a semester.

## Brief user guide
When greeted with ANDIE's interface, you will first need to a open an image before you can access any features. This can be done through a standard CTRL + O command or through our "file" menu. 
From here, your image will be loaded into the interface and you are free to experiment with our many filters and operations.

Users can experiment with our features with confidence knowing that they are non-destructive and can be undone with the click of a button.

> Inside the menu bar

**File** - *Standard file actions, e.g. open, save, save as ...*

**Edit** - *Undo and redo an operation.*

**View** - *Zoom in and out.**

**Filter** - *See your image through a new lense with a selection of pixel configuration surprises.* 

**Colour** - *Splash your image with colour from a selection of pixel altering colour operations.*

**Image** - *Flip, rotate, resize and mirror your image to your hearts delight!*

**Pen** - *Select your colour and pen size and freehand draw on your image with our pen feature.*

**Insert Shape** - *Choose from one of three shapes to insert onto the image. This feature supports a wide range of colours and choose between an outline of the shape or have it filled in.*

**Language** - *Change the language of the application. In this menu you will be able to reload ANDIE as a different language.*

**Crop** - *Click once to enter crop mode, select regions and view the preview before proceeding. Cancel at any time.*

**Macro** - *Begin and end recording of macros simply by click of a button. Once finished you can easily save the macro as a   .ops file to load in later.*

## Known issues/bugs

- The JSpinner object used for when the user needs to input a radius, kernal or zoom size cannot detect characters. If characters are inputed in the wheel radius, then they are ignored.

- If the user inputs a large value that cannot be parsed by <code>Integer.parseInt()</code> the filter will be applied with the maximum radius size 10. In this case there is a delay between the filter being applied and the error message appearing.

- Image export only works if the appropriate file type is specified (Accepted file types: <code>.jpeg/</code> <code>.jpg/</code> <code>.png</code>).

## Running

> Using the JAR file

First navigate to directory containing Andie.jar. 

Run using Powershell: <code>java -jar Andie.jar 2> $null</code>

Run using Git Bash: <code>java -jar Andie.jar 2>/dev/null</code>

Or just run: <code>java -jar Andie.jar</code> (some errors are dumped in terminal but program appears to work fine).
