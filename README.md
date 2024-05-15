# Email_Analysis-
Email analysis is a critical task performed by Security Operations Center (SOC) analysts to identify and mitigate potential cyber threats, especially phishing attacks. Here's a brief overview of my Email analysis process:
![Screenshot 2024-05-14 151826](https://github.com/TikvaAlayo/Email_Analysis-/assets/105614307/73b3f36a-049c-4e9f-93bf-9ff51e8bc05e)
Data Collection: Gather all relevant emails from https://blueteamlabs.online/home/challenge/the-planets-prestige-e5beb8e545 senario for analysis, including.

Email content:

Delivered-To: themajoronearth@gmail.com
Received: by 2002:a92:bd02:0:0:0:0:0 with SMTP id c2csp3604485ile;
        Mon, 25 Jan 2021 22:41:18 -0800 (PST)

 ARC-Authentication-Results: i=1; mx.google.com;
       spf=fail (google.com: domain of billjobs@microapple.com does not designate 93.99.104.210 as permitted sender) smtp.mailfrom=billjobs@microapple.com

Received-SPF: fail (google.com: domain of billjobs@microapple.com does not designate 93.99.104.210 as permitted sender) client-ip=93.99.104.210;
Authentication-Results: mx.google.com;
       spf=fail (google.com: domain of billjobs@microapple.com does not designate 93.99.104.210 as permitted sender) smtp.mailfrom=billjobs@microapple.com
Received: by localhost (Postfix, from userid 33)
	id 1993E221F8; Tue, 26 Jan 2021 01:41:18 -0500 (EST)
To: themajoronearth@gmail.com
Subject: A Hope to CoCanDa
From: "Bill" <billjobs@microapple.com>
X-Priority: 3 (Normal)
Importance: Normal
Errors-To: billjobs@microapple.com
Reply-To: negeja3921@pashter.com 
MIME-version: 1.0
Content-Type: multipart/mixed; boundary=BOUND_600FB98E0DCEE8.49207210
Message-Id: <20210126064118.1993E221F8@localhost>
Date: Tue, 26 Jan 2021 01:41:18 -0500 (EST)  




Body Examination: Examine the email body content details, clues, patterns, or anomalies that may indicate malicious intent or other relevant information to verify the true source of the email, detect phishing attempts, or trace the email's path as i found out "Replay to" email and "from email" showed discrpancy leading to a suspicious email.

Attachment Handling: two PDF files attachments were associate with the email. after analyis by using base64 decoding 4 first bytes were showing it was an zip file after byte analysis at  FILE SIGNATURES TABLE at  https://www.garykessler.net/.
Decrypted zip attacment using Cyberchef : ![Screenshot 2024-05-14 171500](https://github.com/TikvaAlayo/Email_Analysis-/assets/105614307/86b89c48-6bb3-456e-a037-3e651fe3af7f)

Pattern Recognition: patterns in email content, sender behavior, metadata that could indicate suspicious activity and compliance issues.

Insights and Action: Based on the analysis findings, necessary steps were taking by blocking sender IP, such as blocking malicious senders, educating users.

findings: based on exiftool.com found the name of the sender and LocalHost "emkei.c2" which is scam email.

![Screenshot 2024-05-14 171128](https://github.com/TikvaAlayo/Email_Analysis-/assets/105614307/dda885c2-38dc-4a52-9605-131b462ca1a0)

