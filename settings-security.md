# Security Settings

The security tab contains all settings to make your signups more secure against bots.

?>Test this page on [our demo](https://demo2.mailster.co/wp-admin/edit.php?post_type=newsletter&page=mailster_settings#security).

Setting | Purpose
--- | ---
Check MX Record | Mailster tries to get the MX record of the domain from the signup and rejects it if there's no MX record.
Validate via SMTP | Mailster attempts to send a mail to the email address via SMTP (without actually sending it) and reject the signup if it was unsuccessful.
Honeypot | Mailster includes an invisible form element in the signup form which only get filled by bots.
IP Check | Mailster checks if a pending subscriber with the same IP address is already in your database and rejects the signup attempt.
Antiflood | Users must wait at least the given seconds for an additional signup.
Disposable Email Provider | Disallow the usage of email addresses from "throw-away-email-addresses".
Blocked Email Addresses | Define specific email addresses which should get blocked.
Blocked Domains | Define specific domains which should get blocked.
Blocked IP Addresses | Define specific IP addresses or ranges which should get blocked.
Save Domains | Define certain domains which should bypass the above restrictions.


![General Settings Screen](/assets/settings-security.png)
