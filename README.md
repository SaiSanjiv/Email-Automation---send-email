# EXP 10: Email Automation - send email
## AIM

The objective is to establish a connection with the Gmail SMTP server using secure credentials (App Password) and successfully send a test email to a specified recipient.

---

## PROCEDURE

The workflow uses the `UiPath.Mail.Activities` package and the **Send SMTP Mail Message** activity:

1.  **Prerequisites:** A **Gmail App Password** must be generated and used as the `Password` credential, as standard passwords often fail with two-factor authentication enabled.
2.  **Configuration:** The activity is configured with the following standard Gmail SMTP settings:
    * **Host:** `smtp.gmail.com`
    * **Port:** `587`
    * **SecureConnection:** `StartTls`
3.  **Content:** The `From`, `To`, `Subject`, and `Body` properties are set to define the email's content and routing.

---

## OUTPUT

The automation produces the following result:
<img width="1276" height="645" alt="image" src="https://github.com/user-attachments/assets/7c0bf2ee-a292-43a1-bad1-08923e977701" />


* The recipient receives an email in their inbox.
* <img width="1517" height="541" alt="image" src="https://github.com/user-attachments/assets/a947f307-39ff-4020-8808-01739913dbef" />

* The email is tracked in the sender's "Sent Mail" folder.
* <img width="1547" height="774" alt="image" src="https://github.com/user-attachments/assets/34cd3002-ae28-467e-a2fe-0322079b0ee6" />


---

## RESULT

The automation successfully authenticates and communicates with the external Gmail SMTP server, done successfully.
