<b>Assigning File Permissions in Linux</b></br>
As a cybersecurity analyst, I have been tasked to examine existing permissions on the file system. This means that I need to determine if the permissions match the authorization that should be given. If they do not match, I’ll need to modify the permissions to authorize the appropriate users and remove any unauthorized access.

<b>Checked file details</b></br>
The command I used to check file details is: ls 

![image](https://github.com/NATASHASAINI/Linux-permissions/assets/156629309/a2b30663-3adb-465c-a6fa-3888dad14f37)

<b>Permissions String Described</b></br>
In the /home/mobaxterm/desktop/projects , there are five files with the following names and permissions:</b></br>

● project_k.txt.txt ○ User = read, write, ○ Group = read, write ○ Other = read, write

● project_m.txt.txt ○ User = read, write ○ Group = read ○ Other = none

● project_r.txt.txt ○ User= read, write ○ Group = read, write ○ Other = read

● project_t.txt.txt ○ User = read, write ○ Group = read, write ○ Other = read,write

● .project_x.txt.txt ○ User = read, write ○ Group = write ○ Other = none


<b>Changed file permission</b></br>

From the /home/mobaxterm/desktop/projects to display the list of files I used the command ls -l and to remove the write permission on other I used the command 


<b>Changed file permission on a hidden file</b></br>
To assign proper authorization for the hidden file I used the commands as mentioned below:</b></br>

<b>chmod u-x,g+r,g+w,g-x,o+w,o-x project_k.txt .txt</b></br>

![image](https://github.com/NATASHASAINI/Linux-permissions/assets/156629309/79486fff-d001-4d74-815b-906c14ed7e7a)

<b>chmod u-x,g-w,o-r project_m.txt .txt</b></br>

![image](https://github.com/NATASHASAINI/Linux-permissions/assets/156629309/765866aa-c4bc-4cb3-be27-3ea8b7ea4d9c)

<b>chmod u-x,g+w,g+r,o+r project_r.txt .txt</b></br>

![image](https://github.com/NATASHASAINI/Linux-permissions/assets/156629309/80f403c7-1240-402c-afe0-a9b37a17f950)

<b>chmod u-x,g+w,g+r,o+r,o+w project_t.txt .txt</b></br>

![image](https://github.com/NATASHASAINI/Linux-permissions/assets/156629309/9784443f-b120-412f-86e2-0fb74f9091ef)

<b>chmod u-x,g+w,g+r,project_x.txt .txt</b></br>

![image](https://github.com/NATASHASAINI/Linux-permissions/assets/156629309/57777e26-80eb-4689-9f97-4e7d9d825c74)

<b>Conclusion:</b></br>

As required the permissions are authorized on the files
● project_k.txt.txt ○ User = read, write, ○ Group = read, write ○ Other = read, write

● project_m.txt.txt ○ User = read, write ○ Group = read ○ Other = none

● project_r.txt.txt ○ User= read, write ○ Group = read, write ○ Other = read

● project_t.txt.txt ○ User = read, write ○ Group = read, write ○ Other = read,write

● .project_x.txt.txt ○ User = read, write ○ Group = write ○ Other = none

![image](https://github.com/NATASHASAINI/Linux-permissions/assets/156629309/d4dbeca5-1c25-4383-950c-f1553fa3e662)


<b>Summary</b></br>

I reviewed and modified permissions to authorize the appropriate users and remove any unauthorized access to files using the Linux command line. I changed the permission to certain owners and ensured unauthorized access was reviewed and corrected.
