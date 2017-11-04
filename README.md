# sending_gmail

sending_gmail is a simple way for sending text e-mails through Gmail API from your python script. Simply import send_gmail function, and use it to 
send emails on behave of you gmail account.


First register your app via gmail API console.
You can follow these instructions: https://www.epilis.gr/en/blog/2016/07/18/sending-e-mails-using-gmail-api/

send_gmail uses the scope : 'https://console.developers.google.com', it meanse you will be asked to authorize your app, 
for sending messages only. 

Make .client_secret directory in ~ ($HOME) and place there client_secret.json from google api console. 


PLEASE NOTE!!: it is important to name json file exactly: client_secret.json
 
Install sending_gmail package via pip:

pip install sending_gmail


( Please check echo $PYTHONPATH, if it is not setup correctly, especially with Anaconda, python will not find 
the package. You can simply add: 

export PYTHONPATH=/Users/<your username>/anaconda3/bin:$PYTHONPATH

in your ~/.bashrc file

You import this send_gmail function in your script:

import send_gmail from send_gmail

After that you can use your function as:

send_gmail('sender@gmail.com','receipt@some_domain','subject_any_text','message text')

for sender you need to use gmail registered in Google API Console. 




