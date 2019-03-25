# Newsletter Homepage
If you activate the plugin you have to create a new homepage for the newsletter. This page handles subscribes and unsubscriptions.

?>Test this page on [our demo](https://demo.mailster.co/wp-admin/post.php?post=1&action=edit).

!> This page must be linked on the settings page "Frontend".

This is the content of this page:

```html
[newsletter_signup]Signup for the newsletter[newsletter_signup_form id=1][/newsletter_signup]
[newsletter_confirm]Thanks for your interest![/newsletter_confirm]
[newsletter_unsubscribe]Do you really like to unsubscribe?[/newsletter_unsubscribe]
```
There are four shortcode in use:

**`[newsletter_signup]`**

The content of this shortcode is displayed if the user regular visits the page. By default it includes the `[newsletter_signup_form]` shortcode.

**`[newsletter_signup_form]`**

This displays the signup form which can be defined on the settings page. You can add and "id" attribute to use a different form `[newsletter_signup_form id=123]`.

**`[newsletter_confirm]`**

This content is displayed if the new subscriber confirms its email address and clicks on the link in the email.

**`[newsletter_unsubscribe]`**

This content is displayed before the unsubscribe form is displayed. The unsubscribe form is a single email input field or only a button if the user clicks the unsubscribe ink from a campaigns newsletter. You can add `/unsubscribe` to the URL to see this content.