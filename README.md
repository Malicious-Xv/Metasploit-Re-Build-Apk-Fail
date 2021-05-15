Metasploit-Re-Build-Apk-Fail

May Face this issue when binding metasploit payload with large apks

<b>ERROR</B>
<p align="left">
   <img src="https://raw.githubusercontent.com/Malicious-Xv/Metasploit-Re-Build-Apk-Fail/main/Screenshot%20(142).png" width=950px height=550px>
   </p>

<B>SOLUTION</B>

A "method index issue" is exactly what having too many methods will cause :). If you have too many methods, then the method index can't fit into an unsigned 16-bit value, and this is the error that you get.

To solve this Just create another smali folder eg... `smali_classes2` and move your metasploit smali files there ...Thats it..
