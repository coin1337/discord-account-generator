# discord-account-generator
automatically creates discord accounts, no captcha API key required


## info

a script that automates creating discord accounts. it shows how accounts can be created automatically without the user typing unless there is a captcha (h-captcha just needs to be clicked) . it automatically verifies your discord account via email for you and automatically saves the login info in login.txt in email:password:token format. this is used for educational purposes only.


## chromedriver

if chrome doesn't open/crashes, try getting the latest version of chromedriver.exe here > https://chromedriver.chromium.org/downloads. replace the current chromedriver.exe in the folder with the latest version you have downloaded

make sure your chromedriver.exe file is the same version as your current chrome web browser version. to check your current chrome version, paste chrome://settings/help in chrome.


## acc disable bypass (bypass phone number)
reason: temporary email / bot activity detected when joining a server

there is a 70% chance that your account will get disabled when you try joining a server. this happens because discord detects suspicious activity when the temporary email is used.

to bypass this, you should not join any server using the temporary email

after running discord account generator and verifying your email, go to your discord account settings and temporarily change the generated account's email to a legitimate one. (a real gmail account will do; temporary only) after doing so, join any server of your choice. (remember that you cannot join any server using the temporary email or else it will get disabled). after that change back to the temporary email before, and to re-verify again, go to https://www.gmailnator.com/inbox/# + the email that was used previously . for example, to access the temp email, you do https://www.gmailnator.com/inbox/#ran.do.me.mail@gmail.com.


## features
• auto scrape email

• random username from list

• random password

• random date

• auto-email-verify

• automatically get discord token and other login info

• proxy support

• multi-threading

## usage 
you can customize usernames by editing the usernames in discord_usernames.txt.
run the file and use normal mode if you are a inexperienced with proxies and theading.

## python
if you don't have python installed, download python 3.7.6
and make sure you click on the 'add to path' option during
the installation.

### run via python
1. install the required modules
```
pip install selenium
pip install undetected-chromedriver
pip install colorama
pip install bs4
pip install lxml
pip install requests
```
2. to run the script
```
python discordgenerator.py
```

#### proxy support
- if you want to use proxies, simply paste the proxies in config/proxies.txt.  if you want to stop using proxies, just remove all the proxies from the .txt file. the script automatically checks for proxies on startup. http proxies are only supported as of now. if the proxies are not alive, the script will throw a webdriver error.

#### threading mode 
- uses multiple chrome windows
- only run this when you have proxies or else one of you chrome windows will get rate limited.
- do put more than 6 threads unless you think your pc can handle it. i recommend using 2-3 threads.

#### no threading
- this only uses one chrome window. 

#### faq
where can i found my generated accounts?

1. it is located in the output folder. open up login.txt to see the accounts 
that has been generated.
