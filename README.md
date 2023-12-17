  <h3>HOMELAB IN AWS<h3>

  


<h3>Description</h3>

  This home lab project reflects the ability to simulate and respond to security incidents, ensuring compliance with industry standards and best practices. Additionally, the use of multi-factor authentication underscores proficiency in access control practices, while the implementation of encryption mechanisms highlights awareness of data security and privacy considerations in a cloud context.



<h3>Utilities Used</h3>

     - AWS Community Edition
     
     - DUO by Cisco

<h3>OS Environments Used </h3>

    CentOS Stream 9 (x86_64)

<h3>Project walk-through</h3>


    1.) Initial Setup and Account Creation:

    In order to create a home lab in AWS, I needed to create a root-user account. I went ahead and created a free tier AWS account with my personal information.

<br />
    <p align="center">
Enter my information to create an AWS account: <br/>

<img src="https://i.imgur.com/hS0wjMM.png" height="80%" width="80%" alt="AWS HomeLab"/>
<br />
<br />
    <p align="center">
Login to my AWS account using the credentials I signed up with: <br/>

<img src="https://i.imgur.com/pRdZvvd.png" height="80%" width="80%" alt="AWS HomeLab"/>
<br />

    2.) Enable MFA (Multifactor Authentication):

    Multifactor authentication is an additional layer of security protection that I wanted for my root account.

<br />
    <p align="center">
From my console, I click the "Services" button in the top left corner. I select "Security, Identity & Compliance", then I scroll down and click on "IAM". I favorite it so it's easier to acccess later: <br/>
<img src="https://i.imgur.com/gpv3BJm.png" height="80%" width="80%" alt="AWS HomeLab"/>
<br />
<br />
    <p align="center">
Once I'm in the screen for "IAM", I am going to click on the button in the middle of the screen that says, "Add MFA": <br/>
<img src="https://i.imgur.com/xbt43Lx.png" height="80%" width="80%" alt="AWS HomeLab"/>
<br />
<br />
    <p align="center">
Here, I am naming my MFA device and choosing to authenticate with a token from an app called "DUO" by Cisco. Once I finish naming my device and selecting how I'd like to be authenticated into my root-user account, I click the "Next" button in the lower right corner of the screen: <br/>
<img src="https://i.imgur.com/QzeLFKv.png" height="80%" width="80%" alt="AWS HomeLab"/>
<br />
<br />
     <p align="center">
Here, AWS will show me a QR code that I can scan within the authentication app installed on my phone. I will then enter the two TOTP MFA codes that show up sequentially, one after the other, in DUO. Once I confirm the two TOTP MFA codes in the blank fields, I click on the "Add MFA" button on the bottom right of the page, and have officially added another layer of security to protect my root-user account in AWS: <br />
<img src="https://i.imgur.com/jxky0o3.png" height="80%" width="80%" atl="AWS HOmeLab"/>
<br />

    3.) Create + Configure a Billing Alarm:

    In my case, I'm using AWS Community Edition (the free one because I'm a broke student, not an enterprise), but I'm still going to show you how to create a billing alarm anyways. This will ensure that you are notified when your charges for using AWS's cloud services exceed a certain value. (It's really up to you! You can configure the settings to whatever suits your needs)
