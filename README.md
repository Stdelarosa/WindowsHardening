<h1>Windows Hardening</h1>

<h2>Description</h2>
This project was intended to harden my system to protect against potential threats and vulnerabilities as well as malware attacks.
<br />

<h2>Sections</h2>

  - <b>Deleting unused programs and files</b>
  
  - <b>Optimizing Windows Defender</b>
    
  - <b>3rd Party Firewall Configuration</b>

<h2>Deleting Unused Programs and Files</h2>

To begin hardening my system, I begin by deleting unused programs via the Control Panel. I uninstalled 29 programs, now I'm going into my program files to ensure those files were deleted when the programs were uninstalled. The reason for uninstalling unused programs is because it's likely the unused program will be forgotten by the user and there could be a security risk by not keeping the program up to date. It's also a common practice to prevent slowing down a system.
<br />

<h2>Optimizing Windows Defender</h2>

I installed ConfigureDefender which allows me to configure the built-in Defender on Windows 11. By default Defender has most settings disabled, I selected the High protection level which changed the following settings. 

PUA Protection - ON

Cloud Protection Level - Highest

Cloud Check Time Limit - 20s

Productivity apps:

Block Win32 API calls from Office macros - ON

Block Office applications from creating child processes - ON

Block Office applications from creating executable content - ON

Block Office applications from injecting into other processes - ON

Block Adobe Reader from creating child processes - ON

Script Rules:

Block JS/VBS from launching downloaded executable content - ON

Block execution of potentially obfuscated scripts - ON

Email Rules:

Block only Office communication applications from creating child processes - ON

Block executable content from email client and webmail - ON

There are the "Interactive" and "Max" protection levels but I opted against those options because I wanted to avoid too many false positives and the blocking of legitimate software. Of the settings changed, I was most alarmed by the Script Rules being turned off since that's how a lot of malware spreads in a system.
<br />

<h2>3rd Party Firewall Config</h2>

My chosen firewall is Portmaster, it's important to  me that many if not all of the resources I use are free, open-source, and user-friendly which is what led me to choose Portmaster. 

Setting up Portmaster was simple following the quick set-up guide. I noticed Boom 3D, my audio equalizer, trying to make Outgoing connections using TCP. Although I'm certain the connections are checking for updates for the software, I felt the number of connections was alarming and therefore should be blocked seeing as it didn't interfere with its functionality. 
<br />

<h2>Conclusion</h2>
In summary, this project aimed at optimizing the security and performance of my system has proven successful in its multifaceted approach. The initial cleanup involved removing 29 unused programs, a vital step in minimizing potential security vulnerabilities and preventing system sluggishness. The subsequent integration of ConfigureDefender elevated the security posture by fine-tuning Windows Defender settings, with a keen focus on Script Rules to counteract malware threats. The strategic selection of Portmaster as the firewall reinforced the commitment to free, open-source, and user-friendly solutions. Noteworthy was the decision to block outgoing connections from Boom 3D, reflecting a judicious balance between security precautions and preserving system functionality. Collectively, these measures ensure a resilient, secure, and efficiently operating digital environment.
