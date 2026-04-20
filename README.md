# Canon-Pixma-IP6600D
Software and 3D printed replacement parts for the Canon Pixma IP6600D.

## Resources
- http://pixma-faq.periastron.com/

  This resource was **invaluable**. It's only available on [archive.org](http://web.archive.org/web/20080105035258/http://pixma-faq.periastron.com/)

  I've created an [HTTrack backup](pixma-faq/index.html) of this archived website for safe keeping.

- https://www.thingiverse.com/thing:5336201
  
  This made creating the disk tray much easier as this card tray had most of the difficult features already completed.

  This repo has a [backup of the model](parts/card%20tray/PIXMA%20IP6600D%20Card%20Tray%20-%205336201.zip) for safe keeping.

# Replacement Parts
> [!TIP]
> All parts should be printed slowly with a 0.16mm layer height for best results.\
> My parts are designed with this layer height in mind. 

## Card Tray
The only pre-existing part I could find for this printer was the PVC card tray on Thingiverse. I've included it in this repo for archival purposes.

It was only available as a STL, so I used FreeCAD to convert it into a STEP file. This is also included in the repo.

![Card Tray (Parametric)](parts/card%20tray/card%20tray.png)

## Disk Tray
From this card tray, I created the elusive CDR disk tray based on the specifications found [here](https://web.archive.org/web/20080101103419/http://pixma-faq.periastron.com/3.html).

![Disk Tray (Parametric)](parts/disk%20tray/disk%20tray.png)

## SD Card Door
My printer had a broken SD card door, so I recreated it as well. Unlike the original, there is no window on the door. I will probably never use the card reader feature, but I wanted my printer to look nice.

![SD Card Door (Parametric)](parts/sd%20card%20door/sd%20card%20door.png)

## Automatic Slot Feeder (Paper Input) Tray
The hinge was broken on my paper input tray so I recreated the entire tray. I realized it was also missing the paper straightening flap that (apparently) automatically folds out. I recreated this flap from a few pictures, included in the repo now, I was able to find online. I also recreated the sliding extension piece so I had a 100% complete recreation of the entire paper input tray.

For the straighening/alignment flap you need a 1.5mm DIA x 10mm L metal rod and a torsion spring. The model uses McMaster-Carr Part # 9271K644 for the spring, which has a 1.7mm shaft DIA and ~9.5mm length length. 


![Automatic Slot Feeder (Paper Input) Tray (Parametric)](parts/automatic%20slot%20feeder/automatic%20slot%20feeder%20tray.png)

# Software
The **latest** fully featured print driver available from Canon only supports Windows 7 32-bit. There are a few 64-bit drivers that I've tested on Windows 11 and none of them work.

The easiest way to deal with this is to create a Windows 7 32-bit virtual machine. After installing the driver you can use USB passthrough to access it from the virtual machine. 

I used Microsoft's IE9 (or IE10) Windows 7 virtual machine image. You can find more details here:
https://github.com/magnetikonline/linux-microsoft-ie-virtual-machines

After importing the OVA into your virtual machine software (i.e. VirtualBox), you can activate it with [massgrave.dev](https://massgrave.dev/) using the tradition (offline) activation method.

## Driver
Next, install the [Canon IP6600D Print Driver](software/ip6600dvst200ej.exe). I selected the Europe region during install, but this shouldn't matter.

## CD Label Software
For printing the lables, I used the [Canon-provided CD-LabelPrint V1.0.2 software](software/CD-LabelPrint.Win.V1.0.2_E.exe).

## Acrobat Reader
I also installed [Acrobat Reader 9.4.0](software/9.4.0_AdbeRdr940_en_US.exe) so I could print PDF documents.
