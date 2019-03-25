# Authentication Settings

?>Test this page on [our demo](https://demo.mailster.co/wp-admin/edit.php?post_type=newsletter&page=mailster_settings#authentication).


Setting | Purpose
--- | ---
SPF Domain | The domain you would like to add a SPF record. (This is just a helper and has no effect on your email)
DKIM | enable DKIM signed emails (not required if your ESP signs DKIM)
DKIM Domain |The domain you have set the TXT namespace records
DKIM Selector | The selector is used to identify the keys used to attach a token to the email
Keys | If you have defined the domain and a selector you have to generate a public and a private key. Once created you have to add some TXT namespace records at your mail provider. DKIM often doesn't work out of the box. You may have to contact your email provider to get more information. Changing namespace entries can take up to 48 hours to take affect around the world.. It's recommend to change the keys occasionally. If you change one of the settings above new keys are required. Some providers don't allow TXT records with a specific size. Choose less bits in this case.

![Authentication Settings Screen](/assets/settings-authentication.png)
