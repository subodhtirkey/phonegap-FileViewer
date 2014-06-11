phonegap-FileViewer
===================
## File Viewer plugin for Phonegap ##
A plugin that open files like pdf, flv , mp4 and jpg from sdcard in phonegap application.

## Steps to add plugin to your project ##
1. Move fileViewer.js to project's www folder and add reference to the html file. 
2. Create a folder called 'com/phonegap/plugin/' within your project's src/ folder.
3. And copy the Echo.java file into that new folder.
4. Add the following to res/xml/config.xml file `<plugin name="Echo" value="com.phonegap.plugin.Echo"/>`

## Next Steps ##

In FileViewer.js enter the path of the file in your sdcard

    function myshow() {
        window.echo("/sdcard/download/cc.pdf", function (returnvalue) {
            alert(returnvalue); 
        });
    }


Then call the myshow() function in this way from your html file

          <a href="#" onclick="myshow()">open file</a>

  
