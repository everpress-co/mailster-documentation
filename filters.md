# Filters
Mailster provides various hooks and filters you can use to alter the behavior of the plugin or write your own add-ons and extensions. We recommend to read more about hooks on the [official site](https://developer.wordpress.org/plugins/hooks/).

!>  While there are more hooks in the plugin we only list a few here.<hr>

#### `mailster_rewrite_rules`

###### **Filters Mailster specific rewrite rules**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$rules` | `array` | rewrite rules as assoc array

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/tree/master/./classes/frontpage.class.php)[[83](https://github.com/evrpress/mailster/tree/master/./classes/frontpage.class.php#L83-L88)]<br>

#### `mailster_click_target`

###### **Filters the target of the clicked link of a campaign**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$target` | `string` | The target link
`$campaign_id` | `int` | Form The ID of the campaign
`$subscriber_id` | `int` | Form The ID of the subscriber
`$campaign_index` | `int` | The index of the link

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/tree/master/./classes/frontpage.class.php)[[347](https://github.com/evrpress/mailster/tree/master/./classes/frontpage.class.php#L347-L355)]<br>

#### `mailster_redirect_to`

###### **Filters the redirection target after clicking a link in a campaign**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$redirect_to` | `string` | The redirect link
`$campaign_id` | `int` | Form The ID of the campaign
`$subscriber_id` | `int` | Form The ID of the subscriber
`$campaign_index` | `int` | The index of the link

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/tree/master/./classes/frontpage.class.php)[[479](https://github.com/evrpress/mailster/tree/master/./classes/frontpage.class.php#L479-L487)]<br>

#### `mailster_confirm_target`

###### **Filters the redirection target after clicking a link in a campaign**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$target` | `string` | The redirect link
`$subscriber_id` | `int` | Form The ID of the subscriber

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/tree/master/./classes/frontpage.class.php)[[651](https://github.com/evrpress/mailster/tree/master/./classes/frontpage.class.php#L651-L657)]<br>

#### `mailster_cookie_time`

###### **Filters the lifetime of the Mailster cookie.**

Default is 3600 seconds ( 1 Minute )

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$timeout` | `int` | timeout in seconds

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/tree/master/./classes/frontpage.class.php)[[1092](https://github.com/evrpress/mailster/tree/master/./classes/frontpage.class.php#L1092-L1099)]<br>

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

Source: [./classes/mail.class.php](https://github.com/evrpress/mailster/tree/master/./classes/mail.class.php)[[142](https://github.com/evrpress/mailster/tree/master/./classes/mail.class.php#L142-L153)]<br>

#### `mailster_server_errors`

###### **Default server errors where campaigns get paused or skipped**

defaults:<br />
`Sender address rejected`

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$default` | `array` | default values

Source: [./classes/mail.class.php](https://github.com/evrpress/mailster/tree/master/./classes/mail.class.php)[[158](https://github.com/evrpress/mailster/tree/master/./classes/mail.class.php#L158-L166)]<br>

#### `mailster_system_errors`

###### **Default System errors where campaigns get paused or skipped**

defaults:<br />
`Not in Time Frame`

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$default` | `array` | default values

Source: [./classes/mail.class.php](https://github.com/evrpress/mailster/tree/master/./classes/mail.class.php)[[171](https://github.com/evrpress/mailster/tree/master/./classes/mail.class.php#L171-L179)]<br>

#### `mailster_inline_css`

###### **Filter to skip inline CSS**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$inline_css` | `bool` | Whenever to enable inline styles or not

Source: [./classes/mail.class.php](https://github.com/evrpress/mailster/tree/master/./classes/mail.class.php)[[580](https://github.com/evrpress/mailster/tree/master/./classes/mail.class.php#L580-L585)]<br>

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

Source: [./classes/campaigns.class.php](https://github.com/evrpress/mailster/tree/master/./classes/campaigns.class.php)[[2266](https://github.com/evrpress/mailster/tree/master/./classes/campaigns.class.php#L2266-L2301)]<br>

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
Source: [./classes/queue.class.php](https://github.com/evrpress/mailster/tree/master/./classes/queue.class.php)[[438](https://github.com/evrpress/mailster/tree/master/./classes/queue.class.php#L438-L446)]<br>

#### `mailster_time_check_value`

###### **Seconds to prevent forms being submitted**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$time_in_seconds` | `int` | the time in seconds (default:4)

Source: [./classes/form.class.php](https://github.com/evrpress/mailster/tree/master/./classes/form.class.php)[[985](https://github.com/evrpress/mailster/tree/master/./classes/form.class.php#L985-L990)]<br>



