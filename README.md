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

## RESULT

The automation successfully authenticates and communicates with the external Gmail SMTP server, done successfully.
