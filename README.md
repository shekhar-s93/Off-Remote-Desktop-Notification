# Disable-Chrome-Remote-Desktop-Notifications

This guide helps users disable the notifications of Chrome Remote Desktop by modifying the remoting_core.dll file. The process involves:

1.  Accessing the target DLL file in the Chrome Remote Desktop program files.
2.  Using a PE viewer tool to edit the file properties, specifically setting the size attributes to zero in a designated section.
3.  Replacing the original DLL file with the modified version to prevent notification pop-ups.
   
Steps:

1.  Visit https://speedtesting.herokuapp.com/peviewer/.
2.  Open remoting_core.dll (found in C:\Program Files (x86)\Google\Chrome Remote Desktop\[version]) in the PE viewer.
3.  Adjust file settings as instructed in the dialog.
4.  Replace the original file with the edited version to disable notifications.
   
1.   Note: This is a technical procedure. Ensure you back up the original DLL file before replacing it.
2.   Note: Troubleshooting:

If the file does not open or you encounter an "Invalid File" error, first download the file and enter the password chromeremotedesktop@32 upon opening. This should resolve access issues.
 
