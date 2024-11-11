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

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/frontpage.class.php)[[77](https://github.com/evrpress/mailster/blob/4.1.5/./classes/frontpage.class.php#L77-L82)]<br>

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

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/frontpage.class.php)[[337](https://github.com/evrpress/mailster/blob/4.1.5/./classes/frontpage.class.php#L337-L345)]<br>

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

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/frontpage.class.php)[[467](https://github.com/evrpress/mailster/blob/4.1.5/./classes/frontpage.class.php#L467-L475)]<br>

<hr>

#### `mailster_confirm_target`

###### **Filters the redirection target after clicking a link in a campaign**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$target` | `string` | The redirect link
`$subscriber_id` | `int` | The ID of the subscriber

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/frontpage.class.php)[[666](https://github.com/evrpress/mailster/blob/4.1.5/./classes/frontpage.class.php#L666-L672)]<br>

<hr>

#### `mailster_cookie_time`

###### **Filters the lifetime of the Mailster cookie.**

Default is 3600 seconds ( 1 Minute )

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$timeout` | `int` | timeout in seconds

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/frontpage.class.php)[[1074](https://github.com/evrpress/mailster/blob/4.1.5/./classes/frontpage.class.php#L1074-L1081)]<br>

<hr>

#### `mailster_editor_tags`

###### **Modify displayed tags in the editbar**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$tags` | `array` | available tags

Source: [./classes/tinymce.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/tinymce.class.php)[[131](https://github.com/evrpress/mailster/blob/4.1.5/./classes/tinymce.class.php#L131-L136)]<br>

<hr>

#### `mailster_workflow_limit`

###### **filter the limit of subscribers per workflow run**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------

Deprecated: addcslashes(): Passing null to parameter #1 ($string) of type string is deprecated in /Users/Xaver/Sites/dev.local/app/public/wp-content/plugins/mailster/.github/wp-documentor/markdown-hook.php on line 62
`10000` |  | 

Source: [./classes/automation.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/automation.class.php)[[615](https://github.com/evrpress/mailster/blob/4.1.5/./classes/automation.class.php#L615-L620)]<br>

<hr>

#### `mailster_workflow_runtime`

###### **filter the max runtime of a workflow**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------

Deprecated: addcslashes(): Passing null to parameter #1 ($string) of type string is deprecated in /Users/Xaver/Sites/dev.local/app/public/wp-content/plugins/mailster/.github/wp-documentor/markdown-hook.php on line 62
`15` |  | 

Source: [./classes/automation.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/automation.class.php)[[622](https://github.com/evrpress/mailster/blob/4.1.5/./classes/automation.class.php#L622-L627)]<br>

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

Source: [./classes/mail.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/mail.class.php)[[150](https://github.com/evrpress/mailster/blob/4.1.5/./classes/mail.class.php#L150-L161)]<br>

<hr>

#### `mailster_server_errors`

###### **Default server errors where campaigns get paused or skipped**

defaults:<br />
`Sender address rejected`

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$default` | `array` | default values

Source: [./classes/mail.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/mail.class.php)[[166](https://github.com/evrpress/mailster/blob/4.1.5/./classes/mail.class.php#L166-L174)]<br>

<hr>

#### `mailster_system_errors`

###### **Default System errors where campaigns get paused or skipped**

defaults:<br />
`Not in Time Frame`

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$default` | `array` | default values

Source: [./classes/mail.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/mail.class.php)[[179](https://github.com/evrpress/mailster/blob/4.1.5/./classes/mail.class.php#L179-L187)]<br>

<hr>

#### `mailster_inline_css`

###### **Filter to skip inline CSS**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$inline_css` | `bool` | Whenever to enable inline styles or not

Source: [./classes/mail.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/mail.class.php)[[589](https://github.com/evrpress/mailster/blob/4.1.5/./classes/mail.class.php#L589-L594)]<br>

<hr>

#### `mailster_do_placeholder`

###### **Filters the replaced content**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------

Deprecated: addcslashes(): Passing null to parameter #1 ($string) of type string is deprecated in /Users/Xaver/Sites/dev.local/app/public/wp-content/plugins/mailster/.github/wp-documentor/markdown-hook.php on line 62
`$this->content` |  | 

Source: [./classes/placeholder.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/placeholder.class.php)[[376](https://github.com/evrpress/mailster/blob/4.1.5/./classes/placeholder.class.php#L376-L381)]<br>

<hr>

#### `mailster_preview_text_fix`

###### **Adds invisible characters after the preheader text also known as "preview text hack"
Read more here: https://www.litmus.com/blog?p=4367
Updated in Sept. 2023 to use the new invisible characters**

defaults:<br />
`true`

**Arguments**

Argument | Type | Description
-------- | ---- | -----------

Deprecated: addcslashes(): Passing null to parameter #1 ($string) of type string is deprecated in /Users/Xaver/Sites/dev.local/app/public/wp-content/plugins/mailster/.github/wp-documentor/markdown-hook.php on line 62
`true` |  | 

**Example**

Disable the preview text hack

```php
add_filter( 'mailster_preview_text_fix', '__return_false' );
```
Source: [./classes/placeholder.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/placeholder.class.php)[[1107](https://github.com/evrpress/mailster/blob/4.1.5/./classes/placeholder.class.php#L1107-L1117)]<br>

<hr>

#### `mailster_block_form_pre_check_validity`

###### **Pre-Filter the validity of the form. If false the form will not be displayed if true it will be displayed.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------

Deprecated: addcslashes(): Passing null to parameter #1 ($string) of type string is deprecated in /Users/Xaver/Sites/dev.local/app/public/wp-content/plugins/mailster/.github/wp-documentor/markdown-hook.php on line 62
`null` |  | 
`$form_id` | `int` | the form id
`$options` | `array` | the options

Source: [./classes/block-forms.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/block-forms.class.php)[[373](https://github.com/evrpress/mailster/blob/4.1.5/./classes/block-forms.class.php#L373-L380)]<br>

<hr>

#### `mailster_time_check_value`

###### **Seconds to prevent forms being submitted**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------

Deprecated: addcslashes(): Passing null to parameter #1 ($string) of type string is deprecated in /Users/Xaver/Sites/dev.local/app/public/wp-content/plugins/mailster/.github/wp-documentor/markdown-hook.php on line 62
`4` |  | 

Source: [./classes/rest-controller/rest.form.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/rest-controller/rest.form.class.php)[[200](https://github.com/evrpress/mailster/blob/4.1.5/./classes/rest-controller/rest.form.class.php#L200-L205)]<br>Source: [./classes/form.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/form.class.php)[[981](https://github.com/evrpress/mailster/blob/4.1.5/./classes/form.class.php#L981-L986)]<br>

<hr>

#### `mailster_block_form_field_errors`

###### **Allow third parties to hook into the form submission errors**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$fields_errors` | `array` | all current error
`$entry` | `array` | the collected user data
`$request` | `object` | the request

Source: [./classes/rest-controller/rest.form.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/rest-controller/rest.form.class.php)[[211](https://github.com/evrpress/mailster/blob/4.1.5/./classes/rest-controller/rest.form.class.php#L211-L218)]<br>

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

Source: [./classes/campaigns.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/campaigns.class.php)[[2570](https://github.com/evrpress/mailster/blob/4.1.5/./classes/campaigns.class.php#L2570-L2605)]<br>

<hr>

#### `mailster_mail_headers`

###### **Filter the headers values which where added to the campaign**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$headers` | `array` | default header values

Deprecated: addcslashes(): Passing null to parameter #1 ($string) of type string is deprecated in /Users/Xaver/Sites/dev.local/app/public/wp-content/plugins/mailster/.github/wp-documentor/markdown-hook.php on line 62
`$campaign->ID` |  | 

Deprecated: addcslashes(): Passing null to parameter #1 ($string) of type string is deprecated in /Users/Xaver/Sites/dev.local/app/public/wp-content/plugins/mailster/.github/wp-documentor/markdown-hook.php on line 62
`$subscriber->ID` |  | 

Source: [./classes/campaigns.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/campaigns.class.php)[[5275](https://github.com/evrpress/mailster/blob/4.1.5/./classes/campaigns.class.php#L5275-L5282)]<br>

<hr>

#### `mailster_autoresponder_grace_period`

###### **Filter the grace period from campaigns to decide the time when user no longer get the campaign.**

default: 604800 (one week)

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$grace_period` | `int` | The grace period in seconds. set to false to disable

Deprecated: addcslashes(): Passing null to parameter #1 ($string) of type string is deprecated in /Users/Xaver/Sites/dev.local/app/public/wp-content/plugins/mailster/.github/wp-documentor/markdown-hook.php on line 62
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
Source: [./classes/queue.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/queue.class.php)[[427](https://github.com/evrpress/mailster/blob/4.1.5/./classes/queue.class.php#L427-L435)]<br>

<hr>

#### `mailster_subscriber_hash`

###### **calcuate the hash for a subscriber. This should NOT be simple md5**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------

Deprecated: addcslashes(): Passing null to parameter #1 ($string) of type string is deprecated in /Users/Xaver/Sites/dev.local/app/public/wp-content/plugins/mailster/.github/wp-documentor/markdown-hook.php on line 62
`$hash` |  | 
`$email` | `\unknown` | 

Source: [./classes/subscribers.class.php](https://github.com/evrpress/mailster/blob/4.1.5/./classes/subscribers.class.php)[[4326](https://github.com/evrpress/mailster/blob/4.1.5/./classes/subscribers.class.php#L4326-L4341)]<br>

<hr>

#### `mailster_cron_simple_output`

###### **Filter the output of the cron page.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------

Deprecated: addcslashes(): Passing null to parameter #1 ($string) of type string is deprecated in /Users/Xaver/Sites/dev.local/app/public/wp-content/plugins/mailster/.github/wp-documentor/markdown-hook.php on line 62
`(bool) preg_match('/curl|wget/i', $user_agent) || isset($_GET['simple'])` |  | 

**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./includes/cron.php](https://github.com/evrpress/mailster/blob/4.1.5/./includes/cron.php)[[33](https://github.com/evrpress/mailster/blob/4.1.5/./includes/cron.php#L33-L40)]<br>



