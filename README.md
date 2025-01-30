<h1>Configuring Authorizations</h1>


<h2>Description</h2>
In this lab, I searched file and directory permissions and changed ownership of files and directories to limit who can access them. Knowing how to set appropriate permissions is imperative to protect sensitive information and maintain the system's security. 
<br />

<h2>Walk-Through</h2>

<p align="center">
Check file and directory details: <br/>
<img src="https://i.imghippo.com/files/uzm3636oN.png" alt="" border="0">
<br />
<br />
Change file permissions:  <br/>
<img src="https://i.imghippo.com/files/iqKG3496Sc.png" alt="" border="0">
<br />
<br />
Describe the permissions string:  <br/>

The 10-character string is a simple way to determine who's authorized to access the file and their specific permissions. The 1st character indicates if the file is a directory (d) or a regular file (-). The 2nd-4th characters indicate the read (r), write (w), and execute (x) permissions for the user. When one of these characters is a hyphen (-) instead, it indicates the user doesn't have this permission. The 5th-7th characters indicate the read (r), write (w), and execute (x) permissions for the group. When one of these characters is a hyphen (-) instead, it indicates the group doesn't have this permission. The 8th-10th characters indicate the read (r), write (w), and execute (x) permissions for other users. When one of these characters is a hyphen (-) instead, it indicates other users don't have this permission.

In the example above, I changed the permissions for the "project_k.txt" file. The updated 10-character string "-rw-rw-r--" shows that the user and group still have read (r) and write (w) permissions. However, other users only have read (r) permission now. None of the users have execute (x) permission.
<br />
<br />
Change file permissions on a hidden file: <br/>
<img src="https://i.imghippo.com/files/twY4797LA.png" alt="" border="0">
<br />
<br />
Change directory permissions:  <br/>
<img src="https://i.imghippo.com/files/JpGf8561E.png" alt="" border="0">
<br />
<br />
<h2>Summary</h2>
I changed several permissions to align with the level of authorization my company wanted for files and directories in the "projects" directory. The first step was using "ls -la" to check the permissions for the directory. This informed my decisions in the following steps. Then I used the "chmod" command a few times to change the permissions on files and directories.</b>
<br />
<br />

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!># AuthorizationConfigurationLab
