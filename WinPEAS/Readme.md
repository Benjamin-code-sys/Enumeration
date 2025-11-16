# WinPEAS Obfuscation

⇒&nbsp;&nbsp; Due to the poplarity of Winpeas amoung adversaries across the globe as an automated enumeration tool. AV engines including windows defender have developed signatures of its detection in in their products

⇒&nbsp;&nbsp; It is therefore very likely that AV will flag its compiled binary immidiatly when it is dropped onto disk.

⇒&nbsp;&nbsp; To avoid this we can leverage two ways:   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• We can use execute it directly into memmory using `ReflectivePEinjection.ps1` powershell script   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• To obfuscate the its source code thorughly before compiling it. We proceed with this method

## WinPEAS Source-Code Obfuscation

⇒&nbsp;&nbsp; AV engines often place signatures and heauristic detection mechanisms on various and numerous location of the malicious binary, to bypass all of this we need to locate all of them and obfuscate each.

⇒&nbsp;&nbsp; As you can imagine this might be both time consuming and risky since it might lead us to break the functionality of the program. Luckly we have a way around this using an automated python script by `h4wkst3r` <a href="https://github.com/h4wkst3r/InvisibilityCloak">InvisibilityCloak</a>

⇒&nbsp;&nbsp; This script obfuscates the entire solution by either `base64`,`rot13`, or `string reverse`. The procudure of how to use the script is illustrated on h4wkst3r's github page highlighted above
