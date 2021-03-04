
1. Upon inspection of elements on the Login page, I found the developer's note. 

![](Images/owaspTask11_0.0.png)

2. Moved to the /assets directory and found the sensitive flat-file "webapp.db".

![](Images/owaspTask11_0.1.png)

3. Downloaded the flat-file and checked it's size in human readable format
* `du -h webapp.db`

![](Images/owaspTask11_0.2.png)

4. Opened the falt file to check it's tables and decided to dump it's contents as it was only a 28kb file.
* `sqlite3 webapp.db`
* `.tables`
* `.dump`

![](Images/owaspTask11_0.3.png)

5. Found the admin's password hash and then cracked the hash to get the plain-text password on [Crackstation](https://crackstation.net).

![](Images/owaspTask11_0.4.png)

6. Logged in as admin and captured the flag. Challenge completed.

![](Images/owaspTask11_0.5.png)

![](Images/owaspTask11_0.6.png)
