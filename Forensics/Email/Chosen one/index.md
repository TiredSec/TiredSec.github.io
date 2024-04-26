# yOu hAvE bEeN cHoSeN

![Chosen one](./Assets/you-have-been-chosen.PNG "chosen")

<p>One day a couple years ago i had revcieved an email claiming "<strong>i hAd bEeN cHoSeN</strong>", it was immediately clear that this was some sort of scam as:<br>
A) i have never been chosen for anything<br>
B) theres no Dicks sporting goods where i live.</p>
<p> So i decided to dig a little deeper into it, but before that i wanted to find out how emails work in the first place</p>

## How Emails Work
<p>1) Emails are constructed and sent using a mail client like outlook or a web app like gmail<br>
2) The mail client sends the message to a MTA (Mail Transfer Agent) which is just the mail server which is running SMTP<br>
3) The MTA locates the the recipient's advertised mail server and sends it along<br>

we can look at the path that the email went through by looking at the <strong>Received</strong> entries
![received](./Assets/received.PNG "received")<br>

What i have found from my own testing is that NAM11-BN8-obe.outbound.protection.outlook.com or rather *.outbound.protection.outlook.com could be the result from the use of email alias in outlook.com, further more there is the case of the missing return-path which i am currently still investiagating and have no answers as of yet.<br>

The absence of X-Mailer header indicates that the email was probably crafterd via a web-based client instead of locally



</p>
