# Filters
Mailster provides various hooks and filters you can use to alter the behavior of the plugin or write your own add-ons and extensions. We recommend to read more about hooks on the [official site](https://developer.wordpress.org/plugins/hooks/).

!>  While there are more hooks in the plugin we only list a few here.

<hr>

#### `mailster_rewrite_rules`

###### **Filters Mailster specific rewrite rules**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$rules` | `array` | rewrite rules as assoc array

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/blob/3.3.13/./classes/frontpage.class.php)[[81](https://github.com/evrpress/mailster/blob/3.3.13/./classes/frontpage.class.php#L81-L86)]<br>

<hr>

#### `mailster_click_target`

###### **Filters the target of the clicked link of a campaign**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$target` | `string` | The target link
`$campaign_id` | `int` | Form The ID of the campaign
`$subscriber_id` | `int` | Form The ID of the subscriber
`$campaign_index` | `int` | The index of the link

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/blob/3.3.13/./classes/frontpage.class.php)[[341](https://github.com/evrpress/mailster/blob/3.3.13/./classes/frontpage.class.php#L341-L349)]<br>

<hr>

#### `mailster_redirect_to`

###### **Filters the redirection target after clicking a link in a campaign**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$redirect_to` | `string` | The redirect link
`$campaign_id` | `int` | Form The ID of the campaign
`$subscriber_id` | `int` | Form The ID of the subscriber
`$campaign_index` | `int` | The index of the link

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/blob/3.3.13/./classes/frontpage.class.php)[[470](https://github.com/evrpress/mailster/blob/3.3.13/./classes/frontpage.class.php#L470-L478)]<br>

<hr>

#### `mailster_confirm_target`

###### **Filters the redirection target after clicking a link in a campaign**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$target` | `string` | The redirect link
`$subscriber_id` | `int` | The ID of the subscriber

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/blob/3.3.13/./classes/frontpage.class.php)[[647](https://github.com/evrpress/mailster/blob/3.3.13/./classes/frontpage.class.php#L647-L653)]<br>

<hr>

#### `mailster_cookie_time`

###### **Filters the lifetime of the Mailster cookie.**

Default is 3600 seconds ( 1 Minute )

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$timeout` | `int` | timeout in seconds

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/blob/3.3.13/./classes/frontpage.class.php)[[1079](https://github.com/evrpress/mailster/blob/3.3.13/./classes/frontpage.class.php#L1079-L1086)]<br>

<hr>

#### `mailster_editor_tags`

###### **Modify displayed tags in the editbar**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$tags` | `array` | available tags

Source: [./classes/tinymce.class.php](https://github.com/evrpress/mailster/blob/3.3.13/./classes/tinymce.class.php)[[139](https://github.com/evrpress/mailster/blob/3.3.13/./classes/tinymce.class.php#L139-L144)]<br>

<hr>

#### `mailster_subscriber_errors`

###### **Default subscriber errors where campaigns do not get paused or skipped**

defaults:<br />
`SMTP Error: The following recipients failed`<br />
`The following From address failed`<br />
`Invalid address:`<br />
`SMTP Error: Data not accepted`

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$default` | `array` | default values

Source: [./classes/mail.class.php](https://github.com/evrpress/mailster/blob/3.3.13/./classes/mail.class.php)[[145](https://github.com/evrpress/mailster/blob/3.3.13/./classes/mail.class.php#L145-L156)]<br>

<hr>

#### `mailster_server_errors`

###### **Default server errors where campaigns get paused or skipped**

defaults:<br />
`Sender address rejected`

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$default` | `array` | default values

Source: [./classes/mail.class.php](https://github.com/evrpress/mailster/blob/3.3.13/./classes/mail.class.php)[[161](https://github.com/evrpress/mailster/blob/3.3.13/./classes/mail.class.php#L161-L169)]<br>

<hr>

#### `mailster_system_errors`

###### **Default System errors where campaigns get paused or skipped**

defaults:<br />
`Not in Time Frame`

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$default` | `array` | default values

Source: [./classes/mail.class.php](https://github.com/evrpress/mailster/blob/3.3.13/./classes/mail.class.php)[[174](https://github.com/evrpress/mailster/blob/3.3.13/./classes/mail.class.php#L174-L182)]<br>

<hr>

#### `mailster_inline_css`

###### **Filter to skip inline CSS**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$inline_css` | `bool` | Whenever to enable inline styles or not

Source: [./classes/mail.class.php](https://github.com/evrpress/mailster/blob/3.3.13/./classes/mail.class.php)[[583](https://github.com/evrpress/mailster/blob/3.3.13/./classes/mail.class.php#L583-L588)]<br>

<hr>

#### `mailster_do_placeholder`

###### **Filters the replaced content**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->content` |  | 

Source: [./classes/placeholder.class.php](https://github.com/evrpress/mailster/blob/3.3.13/./classes/placeholder.class.php)[[371](https://github.com/evrpress/mailster/blob/3.3.13/./classes/placeholder.class.php#L371-L376)]<br>

<hr>

#### `mailster_preview_text_fix`

###### **Adds invisible characters after the preheader text also known as "preview text hack"
Read more here: https://www.litmus.com/blog?p=4367**

defaults:<br />
`true`

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`true` |  | 

**Example**

Disable the preview text hack

```php
add_filter( 'mailster_preview_text_fix', '__return_false' );
```
Source: [./classes/placeholder.class.php](https://github.com/evrpress/mailster/blob/3.3.13/./classes/placeholder.class.php)[[1091](https://github.com/evrpress/mailster/blob/3.3.13/./classes/placeholder.class.php#L1091-L1100)]<br>

<hr>

#### `mailster_campaign_meta_defaults`

###### **Filter the default meta values of new campaigns**

defaults:<br />
`parent_id: null`<br />
`timestamp: null`<br />
`finished: null`<br />
`active: null`<br />
`timezone: mailster_option( 'timezone' )`<br />
`sent: null`<br />
`error: null`<br />
`from_name: mailster_option( 'from_name' )`<br />
`from_email: mailster_option( 'from' )`<br />
`reply_to: mailster_option( 'reply_to' )`<br />
`subject: null`<br />
`preheader: null`<br />
`template: null`<br />
`file: null`<br />
`editor_height: 500`<br />
`lists: null`<br />
`ignore_lists: null`<br />
`autoresponder: null`<br />
`list_conditions: null`<br />
`head: null`<br />
`colors: null`<br />
`track_opens: mailster_option( 'track_opens' )`<br />
`track_clicks: mailster_option( 'track_clicks' )`<br />
`autoplaintext: true`<br />
`webversion: true`<br />
`auto_post_thumbnail: false`<br />
`tags: array()`<br />
`attachments: array()`

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$defaults` | `array` | the default values

Source: [./classes/campaigns.class.php](https://github.com/evrpress/mailster/blob/3.3.13/./classes/campaigns.class.php)[[2328](https://github.com/evrpress/mailster/blob/3.3.13/./classes/campaigns.class.php#L2328-L2363)]<br>

<hr>

#### `mailster_autoresponder_grace_period`

###### **Filter the grace period from campaigns to decide the time when user no longer get the campaign.**

default: 604800 (one week)

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$grace_period` | `int` | The grace period in seconds. set to false to disable
`$campaign` |  | 

**Example**

Adjust to one month

```php
add_filter( 'mailster_autoresponder_grace_period', function( $grace_period_in_seconds, $campaign_id ){
	return MONTH_IN_SECONDS;
},10 , 2 );
```

Disable the grace period

```php
add_filter( 'mailster_autoresponder_grace_period', '__return_false' );
```
Source: [./classes/queue.class.php](https://github.com/evrpress/mailster/blob/3.3.13/./classes/queue.class.php)[[428](https://github.com/evrpress/mailster/blob/3.3.13/./classes/queue.class.php#L428-L436)]<br>

<hr>

#### `mailster_time_check_value`

###### **Seconds to prevent forms being submitted**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$time_in_seconds` | `int` | the time in seconds (default:4)

Source: [./classes/form.class.php](https://github.com/evrpress/mailster/blob/3.3.13/./classes/form.class.php)[[982](https://github.com/evrpress/mailster/blob/3.3.13/./classes/form.class.php#L982-L987)]<br>



