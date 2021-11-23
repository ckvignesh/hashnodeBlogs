## WordPress website hosting using AWS

This article deals with three tasks — creating a WordPress Instance on AWS, A form to add photos and comments and the Security aspects of the website.

This article is divided into three parts. References at the end.

1.  Creation of a Wordpress Instance on AWS
2.  Adding Photos and Comments
3.  Brief instructions on-
4.  How the website is secured
5.  How users will be provided secure access to website
6.  **Creation of a Wordpress Instance on AWS**
7.  Login to the AWS console and go to the Instances menu under EC2 services of AWS console. Click on the “launch instance” option to create the new Wordpress instance. (WPBeginners-WordPress-Tutorials) (Zen)

**Figure 1**

1.  Click on the “AWS Marketplace” in the left window and search for the “Wordpress certified by Bitnami and Automatic option”. Select it and proceed.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652426133/bqh3ZIydr.png)

**Figure 2**

1.  Select the “t2.micro” option which is eligible for free tier and proceed.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652428386/tEOpwNTdt.png)

**Figure 3**

1.  Set the Network to the default VPC, give no preferences to the Subnet and use the subnet setting for the Auto-Assign IP

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652430564/d-0BrxR9f.png)

**Figure 4**

1.  Configure the security group to allow HTTP and HTTPS traffic, so that any user can enter and submit the comments

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652432831/6tiGB4ySk.png)

**Figure 5**

1.  Review the instance before it’s launched

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652435202/-G12HAZUk.png)

**Figure 6**

1.  Download the new key pair after naming it and proceed to create the instance.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652437681/y6tpl7Ah6.png)

**Figure 7**

1.  Wait as the instance is being created.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652439840/y-53KY2wU.png)

**Figure 8**

1.  Now the instance is seen on the list of the instances in our EC2 menu.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652442335/71yzAl0at.png)

**Figure 9**

1.  Click on Actions, Instance Settings and System Log as shown in the figure.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652445457/olYJV8kwg.png)

**Figure 10**

1.  Scroll down to the bottom of the System log page until you see the Setting Bitnami application password. Select it, copy and paste it to a notepad file. This is for future reference.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652447859/iVkGnKgdb.png)

**Figure 11**

1.  Copy the public IP of the instance and save it again, for future reference.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652450250/XjFtAZ4cM.png)

**Figure 12**

Now copy paste the public IP of that instance and see the default Wordpress website that is hosted.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652453179/vlVzfdV9c.png)

**Figure 13**

1.  Scroll down to the bottom of the page and click on the “Login option”

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652455789/ChluDj0hk.png)

**Figure 14**

1.  Enter “user” in the username and the saved password into the password box.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652457921/wDDorJWG8.png)

**Figure 15**

1.  The login is successful!

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652460272/coWxPNRWM.png)

**Figure 16**

1.  **Adding photos and comments under a post.**

Wordpress generally allows the user to accept ordinary string comments from the public. This can be subjected to moderation or approval. Follow these steps to accept picture comments. (WPBeginner-WordPress-Tutorials)

1.  Click on “plug-in” and then search for the DCO Comment Attachment plug-in. Install and activate it.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652462670/N0mfS_4Fh.png)

**Figure 17**

1.  Check its progress in the plug-in list. Now, it has to be configured.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652465630/1sUtSkuFz.png)

**Figure 18**

1.  Go to “Settings” and select the DCO Comment Attachment Settings. The settings have to be configured now.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652467973/EKpqHWCXnP.png)

**Figure 19**

1.  We must allow only images to be posted. Hence, uncheck all the other formats.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652470348/GvurNNKU_.png)

**Figure 20**

1.  Don’t forget to save the settings

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652472546/E2zKGFcY2.png)

**Figure 21**

1.  Now go to the page and edit the layout, caption etc. Under the “Discussion” menu in the right, enable “Allow Comments”.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652475093/hsELXD8EU.png)

**Figure 22**

1.  Now, let’s test the page. Go to the URL after logging out as the administrator.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652477260/UK9AV2TVpW.png)

**Figure 23**

1.  This is the page to add the comment and a photo. Once this is done,

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652479431/gVHsLFpO6.png)

**Figure 24**

1.  Once it’s completed, click on the “Submit” option.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652481519/3RVWy6bsi.png)

**Figure 25**

1.  Now, the uploaded picture and the text of the comment have been submitted for moderation.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652483756/0Lr0xi-o3.png)

**Figure 26**

1.  The comment which was submitted is seen in the bottom, along with the name of the user who sent it.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652485982/NpxKZ5xJx.png)

**Figure 27**

1.  Click on the “Media Library” on the left side to see the media submitted by the user. This gets stored on the Wordpress website.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652488149/cOnYoUV5t.png)

**Figure 28**

1.  **Brief instructions on-**

*   **How the website is secured**
*   **How users will be provided secure access to website**

1.  **How the website is secured:**

The Website has a registration page where the user can request the admin for an account. There is no way for any user to create an ID without the permission of the Administrator. This by itself is the biggest check to prevent the intrusion attempts. The administrator has set strong password policies for the root account and for the user accounts.

The Wordpress Hosting service provides an inbuilt firewall which keeps out most of the unnecessary traffic and ensures scalability along with the security apparatus. Therefore, the identity of the users and the administrator is safe.

1.  **How users will be provided secure access to website:**

This will be done by the Administrator creating a new user ID for the user to enter. Follow the steps to do it. (Balkhi) (WPBeginner-Wordpress-Tutorials)

1.  Search for a user registration plug-in and download it.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652490891/vjIBRPNNE.png)

**Figure 29**

1.  Go to the General settings under the user registration tab (in left menu) and review the default settings.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652493067/r66P2xn-3.png)

**Figure 30**

1.  The Admin is the default user. Click on “Add new” on top to add a new user.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652495260/3XW4rl8iU.png)

**Figure 31**

1.  Set username, their email ID (for password reset), name and password (auto generated). Tick the “send user notification” which sends an email to the user with the creation of the account, where password is encrypted and sent. Confirm and proceed. The

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652497391/cgvAFJwoh.png)

**Figure 32**

1.  Now the new user is added to the list.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652499617/qLsXlmc4P.png)

**Figure 33**

1.  The user has now been able to successfully login to his ID with the credentials provided.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1637652501944/wCgHgAZ9p.jpeg)

**Figure 34**

### References

Balkhi, S. (n.d.). *HOW TO ALLOW USER REGISTRATION ON YOUR WORDPRESS SITE*. Retrieved from WPBeginner: [https://www.wpbeginner.com/beginners-guide/how-to-allow-user-registration-on-your-wordpress-site/](https://www.wpbeginner.com/beginners-guide/how-to-allow-user-registration-on-your-wordpress-site/)

WPBeginners-WordPress-Tutorials. (n.d.). *How to Install a WordPress Plugin (3 Different Methods)*. Retrieved from YouTube: [https://www.youtube.com/watch?v=QXbrdVjWaME&feature=youtu.be](https://www.youtube.com/watch?v=QXbrdVjWaME&feature=youtu.be)

WPBeginner-Wordpress-Tutorials. (n.d.). *How to Allow User Registration on Your WordPress Site*. Retrieved from YouTube: [https://www.youtube.com/watch?v=TuCX5W32Hvg&feature=youtu.be](https://www.youtube.com/watch?v=TuCX5W32Hvg&feature=youtu.be)

WPBeginner-WordPress-Tutorials. (n.d.). *How to Allow Users to Upload Images in WordPress Comments*. Retrieved from YouTube: [https://www.youtube.com/watch?v=UGLj3gt65QU&feature=youtu.be](https://www.youtube.com/watch?v=UGLj3gt65QU&feature=youtu.be)

Zen, O. P. (n.d.). *How to Install WordPress on AWS*. Retrieved from YouTube: [https://www.youtube.com/watch?v=4WR7EFFLF04&feature=youtu.be](https://www.youtube.com/watch?v=4WR7EFFLF04&feature=youtu.be)