# Putty-Ping

Putty-Ping is a ping service for when using putty to check if the connection you're trying to connect to is online, before you create a connection.

## How to configure


1. Download [PuTTY](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)

2. Create a profile in Windows Terminal for your saved putty session <br />
and add a ping service for before you try to enter your session.

First, create a *.putty* folder to your Windows Home Directory and then add the *puttyping.bat* file. <br />
After that you can add this profile to your Windows Terminal .json file.

```json
{
    "commandline": "\"C:\\Users\\Your-Name\\.putty\\puttyping.bat\" Ip-Adress \"Your-Putty-Session\"",
    "guid": "{[Use-Guid-Generator](https://guidgenerator.com/online-guid-generator.aspx)}",
    "icon": "ms-appx:///ProfileIcons/{9acb9455-ca41-5af7-950f-6bca1bc9722f}.png",
    "name": "Name-Showed-In-Windows-Terminal"
}
```

You can also use *plink.exe*, but plink does not give support for the arrow keys, the <br />
escape key, nor the function keys, but in return acts more like an interactive session.

