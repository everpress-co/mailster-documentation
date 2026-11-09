# Filters
Mailster provides various hooks and filters you can use to alter the behavior of the plugin or write your own add-ons and extensions. We recommend to read more about hooks on the [official site](https://developer.wordpress.org/plugins/hooks/).

!>  While there are more hooks in the plugin we only list a few here.

<hr>

#### `mailster_export_fields`

###### **Export subscribers screen.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$fields` | `` | 

Source: [./views/manage/export.php](https://github.com/everpress-co/mailster/blob/4.1.22/./views/manage/export.php)[[2](https://github.com/everpress-co/mailster/blob/4.1.22/./views/manage/export.php#L2-L115)]<br>

<hr>

#### `mailster_verify_new_subscriber`

###### **Runs verification filters on subscriber entry data before insert or update.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`(array) $entry` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[1106](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L1106-L1122)]<br>#### `mailster_verify_subscriber`

###### **Runs verification filters on subscriber entry data before insert or update.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`(array) $entry` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[1106](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L1106-L1124)]<br>

<hr>

#### `mailster_subscriber_rating`

###### **Recalculates engagement rating for the given subscribers.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$rating` | `` | 
`$id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3.8` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[2388](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L2388-L2428)]<br>#### `mailster_form_list_order`

###### **Returns lists assigned to a form.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`false` | `` | 
`$id` | `int` | Form ID.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[1462](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L1462-L1482)]<br>

<hr>

#### `mailster_subscriber_rating_{$id}`

###### **Recalculates engagement rating for the given subscribers.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$rating` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3.8` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[2388](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L2388-L2429)]<br>

<hr>

#### `mailster_subscriber_notification_delay`

###### **Queues or sends an admin notification for a new subscriber.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$timestamp` | `int|null` | Optional schedule timestamp.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[3362](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L3362-L3384)]<br>#### `mailster_subscriber_unsubscribe_notification_delay`

###### **Queues or sends an admin notification for an unsubscribe.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$timestamp` | `int|null` | Optional schedule timestamp.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[3430](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L3430-L3455)]<br>#### `mailster_subscriber_notification_delay`

###### **Sanitizes and validates options submitted via the Settings API before save.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$timestamp` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/settings.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/settings.class.php)[[787](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/settings.class.php#L787-L1167)]<br>#### `mailster_subscriber_unsubscribe_notification_delay`

###### **Sanitizes and validates options submitted via the Settings API before save.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$timestamp` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/settings.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/settings.class.php)[[787](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/settings.class.php#L787-L1184)]<br>

<hr>

#### `mailster_subscribers_get_by_type_sql`

###### **Gets a subscriber by an arbitrary column type and value.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$sql` | `` | 
`$type` | `string` | Lookup column or type name.
`$value` | `mixed` | Value to store or filter.
`$include_deleted` | `bool` | Whether to include deleted subscribers.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[3816](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L3816-L3849)]<br>

<hr>

#### `mailster_comment_post_lists`

###### **Creates a subscriber from a comment submission when the checkbox is set.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$lists` | `` | 
`$comment` | `` | 
`$comment_approved` | `int|string` | Comment approval status.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[4287](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L4287-L4311)]<br>#### `mailster_comment_post_userdata`

###### **Creates a subscriber from a comment submission when the checkbox is set.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$userdata` | `` | 
`$comment` | `` | 
`$comment_approved` | `int|string` | Comment approval status.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[4287](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L4287-L4321)]<br>#### `mailster_comment_post_lists`

###### **Creates a subscriber when a comment is approved and opt-in was requested.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$lists` | `` | 
`$comment` | `` | 
`$comment_approved` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[4336](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L4336-L4358)]<br>#### `mailster_comment_post_userdata`

###### **Creates a subscriber when a comment is approved and opt-in was requested.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$userdata` | `` | 
`$comment` | `` | 
`$comment_approved` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[4336](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L4336-L4369)]<br>

<hr>

#### `mailster_subscriber_hash`

###### **Calculates the subscriber hash for an email. This should not be a simple MD5.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$hash` | `` | 
`$email` | `string` | Email address.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[4759](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L4759-L4776)]<br>#### `mailster_is_email`

###### **Validate an email address beyond is_email().**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`null` | `` | 
`$email` | `string` | Email.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./includes/functions.php](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php)[[1108](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php#L1108-L1118)]<br>

<hr>

#### `mailster_autoresponder_hook_args`

###### **Queues or duplicates an autoresponder campaign when its hook fires.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$query_args` | `` | 
`$campaign_id` | `int` | Campaign ID.
`$subscriber_ids` | `int|array|null` | Subscriber ID or IDs. (optional).
`$args` | `array` | Extra hook arguments used as tags. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[314](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L314-L347)]<br>#### `mailster_autoresponder_hook_args_current_filter()`

###### **Queues or duplicates an autoresponder campaign when its hook fires.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$query_args` | `` | 
`$campaign_id` | `int` | Campaign ID.
`$subscriber_ids` | `int|array|null` | Subscriber ID or IDs. (optional).
`$args` | `array` | Extra hook arguments used as tags. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[314](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L314-L348)]<br>#### `mailster_get_post_list_args`

###### **Returns HTML list markup of posts or media for the campaign post selector.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$args` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/ajax.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php)[[1699](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php#L1699-L1790)]<br>#### `mailster_actions_add_sql`

###### **Inserts or increments a row in the matching action_* table.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$sql` | `` | 
`$args` | `array` | Action fields; must include string type key.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/actions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/actions.class.php)[[267](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/actions.class.php#L267-L295)]<br>#### `mailster_delete_args`

###### **Deletes or trashes subscribers matching list/status/condition args.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$args` | `array` | Query args and job metadata (lists, status, conditions, etc.).

**Changelog**

Version | Description
------- | -----------
`3.1` | 

Source: [./classes/manage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/manage.class.php)[[1592](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/manage.class.php#L1592-L1622)]<br>#### `mailster_freemius_args`

###### **Renders a Freemius checkout button with the configured license context.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$args` | `array` | Optional Freemius checkout arguments.

**Changelog**

Version | Description
------- | -----------
`4.1.5` | 

Source: [./includes/freemius.php](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/freemius.php)[[347](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/freemius.php#L347-L378)]<br>

<hr>

#### `mailster_inline_editor`

###### **Whether the TinyMCE inline editor is enabled for campaign content.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`version_compare('4.6', $wp_version, '<=')` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[2109](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L2109-L2122)]<br>

<hr>

#### `mailster_attachments_max_filesize`

###### **Persists campaign meta, lists, and delivery settings on save_post.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`1024 * 1024` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[2279](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L2279-L2364)]<br>#### `mailster_attachments_max_filesize`

###### **Sends a campaign test email to the requested recipients and returns status JSON.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`1024 * 1024` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/ajax.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php)[[809](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php#L809-L885)]<br>

<hr>

#### `mailster_campaign_meta_defaults`

###### **Filter the default meta values of new campaigns**

Defaults:<br />
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

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[2899](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L2899-L2934)]<br>#### `mailster_send_replace`

###### **Deprecated wrapper to send a notification email.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`wp_parse_args($replace, $defaults)` | `` | 
`$defaults` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./includes/deprecated.php](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/deprecated.php)[[8](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/deprecated.php#L8-L33)]<br>

<hr>

#### `mailster_get_recipients_part`

###### **Builds HTML for a page of campaign recipient rows in the editor.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`1000` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[4991](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L4991-L5012)]<br>

<hr>

#### `mailster_update_metric_columns`

###### **Handles Heartbeat API updates for live campaign progress in admin.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`(array) $_POST['data']['mailster']['columns']` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[5278](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L5278-L5314)]<br>

<hr>

#### `mailster_inline_css`

###### **Sends a campaign email to a subscriber with tracking and tags.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`true` | `` | 
`$campaign->ID` | `` | 
`$subscriber->ID` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[5498](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L5498-L5591)]<br>#### `mailster_inline_css`

###### **Sends a campaign email to a subscriber with tracking and tags.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`true` | `` | 
`$campaign->ID` | `` | 
`$subscriber->ID` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[5498](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L5498-L5659)]<br>#### `mailster_mail_headers`

###### **Filter the headers values which where added to the campaign**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$headers` | `array` | default header values
`$campaign->ID` | `` | 
`$subscriber->ID` | `` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[5816](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L5816-L5823)]<br>

<hr>

#### `mailster_campaign_content`

###### **Sends a campaign email to a subscriber with tracking and tags.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$content` | `` | 
`$campaign` | `` | 
`$subscriber` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[5498](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L5498-L5663)]<br>#### `mailster_campaign_content`

###### **Sends a campaign test email to the requested recipients and returns status JSON.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$content` | `` | 
`get_post($ID)` | `` | 
`$subscriber` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/ajax.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php)[[809](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php#L809-L1021)]<br>

<hr>

#### `mailster_check_for_autoresponder_accepted_status`

###### **Queues a campaign for change processing on status transition.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`'publish'` | `` | 
`$post` | `\WP_Post` | Post being transitioned.

**Changelog**

Version | Description
------- | -----------
`2.4.17` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[5863](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L5863-L5887)]<br>#### `mailster_auto_post`

###### **Returns placeholder pattern data for a single selected post in the campaign editor.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$data` | `` | 
`$post` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/ajax.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php)[[1954](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php#L1954-L2025)]<br>#### `mailster_check_for_autoresponder_accepted_status`

###### **Enqueues published_post jobs when a non-newsletter post reaches an accepted status.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`'publish'` | `` | 
`$post` | `\WP_Post` | Post object after save.

**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/trigger.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/trigger.class.php)[[367](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/trigger.class.php#L367-L391)]<br>

<hr>

#### `mailster_editor_toolbar1`

###### **Returns script and style tags for the campaign editor iframe.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`'bold,italic,underline,strikethrough,|,mailster_mce_button,|,forecolor,backcolor,|,undo,redo,mailster_emoji,|,link,unlink,|,removeformat,|,mailster_remove_element'` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[6311](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L6311-L6363)]<br>

<hr>

#### `mailster_editor_toolbar2`

###### **Returns script and style tags for the campaign editor iframe.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`'fontselect,fontsizeselect|bullist,numlist,|,alignleft,aligncenter,alignright,alignjustify'` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[6311](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L6311-L6364)]<br>

<hr>

#### `mailster_editor_toolbar3`

###### **Returns script and style tags for the campaign editor iframe.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`''` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[6311](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L6311-L6365)]<br>#### `mailster_editor_single_toolbar3`

###### **Returns script and style tags for the campaign editor iframe.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`''` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[6311](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L6311-L6369)]<br>#### `mailster_ical`

###### **Applies Mailster charset, encoding, and SMTP defaults then constructs PHPMailer.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`''` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mail.helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.helper.class.php)[[82](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.helper.class.php#L82-L93)]<br>

<hr>

#### `mailster_editor_single_toolbar1`

###### **Returns script and style tags for the campaign editor iframe.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`'bold,italic,underline,strikethrough,|,mailster_mce_button,|,forecolor,backcolor,mailster_emoji,|,link,unlink,|,removeformat,|,mailster_remove_element'` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[6311](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L6311-L6367)]<br>

<hr>

#### `mailster_editor_single_toolbar2`

###### **Returns script and style tags for the campaign editor iframe.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`'fontselect,fontsizeselect'` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[6311](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L6311-L6368)]<br>

<hr>

#### `mailster_editor_font_formats`

###### **Returns script and style tags for the campaign editor iframe.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`array('System' => '-apple-system,BlinkMacSystemFont,\'Segoe UI\',Roboto,Oxygen-Sans,Ubuntu,Cantarell,\'Helvetica Neue\',sans-serif', 'Arial' => 'arial,helvetica,sans-serif', 'Arial Black' => 'arial black,avant garde,serif', 'Courier New' => 'courier new,courier,serif', 'Georgia' => 'georgia,palatino,serif', 'Helvetica' => 'helvetica,sans-serif', 'Tahoma' => 'tahoma,arial,helvetica,sans-serif', 'Times New Roman' => 'times new roman,times,serif', 'Trebuchet MS' => 'trebuchet ms,geneva,sans-serif', 'Verdana' => 'verdana,geneva,sans-serif')` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[6311](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L6311-L6385)]<br>

<hr>

#### `mailster_form_field_label_{$field_id}`

###### **Builds and optionally echoes the HTML for the current form.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$label` | `` | 
`$field` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/form.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php)[[409](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php#L409-L529)]<br>#### `mailster_conditions_nice_name`

###### **Translates a field, operator, or value token into a display label.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$string` | `string` | Raw token to translate.
`$type` | `string|null` | Context: field, operator, or value. (optional).
`$field` | `string|null` | Related field key for operator/value context. (optional).

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[1137](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L1137-L1219)]<br>#### `mailster_get_condition_field`

###### **Builds a SQL condition fragment for a field, operator, and value.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$field` | `string` | Field key (subscriber, custom, meta, action, etc.).

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/subscriber.query.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php)[[1297](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php#L1297-L1392)]<br>

<hr>

#### `mailster_form_button_as_input`

###### **Builds and optionally echoes the HTML for the current form.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`true` | `` | 
`$this->ID` | `` | 
`$this->form` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/form.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php)[[409](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php#L409-L744)]<br>#### `mailster_form_fields`

###### **Builds and optionally echoes the HTML for the current form.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$fields` | `` | 
`$this->ID` | `` | 
`$this->form` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/form.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php)[[409](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php#L409-L756)]<br>#### `mailster_profile_form`

###### **Builds and optionally echoes the HTML for the current form.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$html` | `` | 
`$this->ID` | `` | 
`$this->form` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/form.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php)[[409](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php#L409-L779)]<br>#### `mailster_unsubscribe_form`

###### **Builds and optionally echoes the HTML for the current form.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$html` | `` | 
`$this->ID` | `` | 
`$this->form` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/form.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php)[[409](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php#L409-L782)]<br>#### `mailster_form`

###### **Builds and optionally echoes the HTML for the current form.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$html` | `` | 
`$this->ID` | `` | 
`$this->form` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/form.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php)[[409](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php#L409-L785)]<br>#### `mailster_pre_submit`

###### **Handles subscribe, update, and unsubscribe POST submissions.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$formdata` | `` | 
`$this->form` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/form.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php)[[1096](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php#L1096-L1162)]<br>

<hr>

#### `mailster_unsubscribe_form`

###### **Renders the unsubscribe form HTML, optionally completing single opt-out.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$html` | `` | 
`$this->campaignID` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/form.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php)[[1027](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php#L1027-L1092)]<br>

<hr>

#### `mailster_time_check_value`

###### **Seconds to prevent forms being submitted**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$time_in_seconds` | `int` | the time in seconds (default:4)

Source: [./classes/form.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php)[[1225](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php#L1225-L1230)]<br>

<hr>

#### `mailster_submit`

###### **Handles subscribe, update, and unsubscribe POST submissions.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->object` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/form.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php)[[1096](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php#L1096-L1238)]<br>#### `mailster_submit_{$this->ID}`

###### **Handles subscribe, update, and unsubscribe POST submissions.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->object` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/form.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php)[[1096](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php#L1096-L1239)]<br>#### `mailster_post_submit`

###### **Handles subscribe, update, and unsubscribe POST submissions.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->object` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/form.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php)[[1096](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php#L1096-L1468)]<br>#### `mailster_post_submit_{$this->ID}`

###### **Handles subscribe, update, and unsubscribe POST submissions.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->object` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/form.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php)[[1096](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/form.class.php#L1096-L1469)]<br>

<hr>

#### `mailster_location_db_folder`

###### **Returns the filesystem path to the GeoLite2 City database file.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`MAILSTER_UPLOAD_DIR` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3.6` | 

Source: [./classes/geo.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/geo.class.php)[[219](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/geo.class.php#L219-L228)]<br>

<hr>

#### `mailster_location_db_file_city`

###### **Returns the filesystem path to the GeoLite2 City database file.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`trailingslashit($folder) . 'geo/GeoLite2-City.mmdb'` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3.6` | 

Source: [./classes/geo.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/geo.class.php)[[219](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/geo.class.php#L219-L230)]<br>

<hr>

#### `mailster_verify_options`

###### **Sanitizes and validates options submitted via the Settings API before save.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$options` | `array` | Submitted options.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/settings.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/settings.class.php)[[787](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/settings.class.php#L787-L1412)]<br>#### `mailster_notification_{$template}_{$filter}`

###### **Supplies default notification field values based on template and current filter.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$content` | `mixed` | Current filter value.
`$subscriber` | `object|null` | Subscriber object when available.
`$options` | `array` | Send options.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php)[[264](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php#L264-L410)]<br>#### `mailster_notification_content`

###### **Builds and sends the notification email for a subscriber and options.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->message` | `` | 
`$template` | `` | 
`$subscriber` | `` | 
`$options` | `array` | Send options including template and field overrides.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php)[[528](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php#L528-L579)]<br>#### `mailster_notification_to`

###### **Builds and sends the notification email for a subscriber and options.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->to` | `` | 
`$template` | `` | 
`$subscriber` | `` | 
`$options` | `array` | Send options including template and field overrides.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php)[[528](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php#L528-L585)]<br>#### `mailster_notification_subject`

###### **Builds and sends the notification email for a subscriber and options.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->subject` | `` | 
`$template` | `` | 
`$subscriber` | `` | 
`$options` | `array` | Send options including template and field overrides.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php)[[528](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php#L528-L586)]<br>#### `mailster_notification_file`

###### **Builds and sends the notification email for a subscriber and options.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->file` | `` | 
`$template` | `` | 
`$subscriber` | `` | 
`$options` | `array` | Send options including template and field overrides.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php)[[528](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php#L528-L587)]<br>#### `mailster_notification_headline`

###### **Builds and sends the notification email for a subscriber and options.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->headline` | `` | 
`$template` | `` | 
`$subscriber` | `` | 
`$options` | `array` | Send options including template and field overrides.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php)[[528](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php#L528-L588)]<br>#### `mailster_notification_preheader`

###### **Builds and sends the notification email for a subscriber and options.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->preheader` | `` | 
`$template` | `` | 
`$subscriber` | `` | 
`$options` | `array` | Send options including template and field overrides.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php)[[528](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php#L528-L589)]<br>#### `mailster_notification_replace`

###### **Builds and sends the notification email for a subscriber and options.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->replace` | `` | 
`$template` | `` | 
`$subscriber` | `` | 
`$options` | `array` | Send options including template and field overrides.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php)[[528](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php#L528-L591)]<br>#### `mailster_notification_from`

###### **Builds and sends the notification email for a subscriber and options.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->mail->from` | `` | 
`$template` | `` | 
`$subscriber` | `` | 
`$options` | `array` | Send options including template and field overrides.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php)[[528](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php#L528-L602)]<br>#### `mailster_notification_from_name`

###### **Builds and sends the notification email for a subscriber and options.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->mail->from_name` | `` | 
`$template` | `` | 
`$subscriber` | `` | 
`$options` | `array` | Send options including template and field overrides.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php)[[528](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php#L528-L603)]<br>#### `mailster_notification_reply_to`

###### **Builds and sends the notification email for a subscriber and options.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`mailster_option('reply_to', false)` | `` | 
`$template` | `` | 
`$subscriber` | `` | 
`$options` | `array` | Send options including template and field overrides.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php)[[528](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php#L528-L604)]<br>#### `mailster_notification_attachments`

###### **Builds and sends the notification email for a subscriber and options.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->attachments` | `` | 
`$template` | `` | 
`$subscriber` | `` | 
`$options` | `array` | Send options including template and field overrides.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php)[[528](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php#L528-L612)]<br>#### `mailster_block_form_pre_check_validity`

###### **Pre-Filter the validity of the form. If false the form will not be displayed if true it will be displayed.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`null` | `` | 
`$form_id` | `int` | the form id
`$options` | `array` | the options

Source: [./classes/block-forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/block-forms.class.php)[[609](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/block-forms.class.php#L609-L616)]<br>#### `mailster_subscribe_button_src`

###### **Builds HTML and loader script for an external subscribe button.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$button_src` | `` | 
`$options` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[1678](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L1678-L1704)]<br>

<hr>

#### `mailster_verify_texts`

###### **Filters submitted texts and optionally reloads defaults from a language file.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$texts` | `array` | Submitted text strings.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/settings.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/settings.class.php)[[1418](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/settings.class.php#L1418-L1447)]<br>

<hr>

#### `mailster_system_info`

###### **Builds a labeled system information dump for support diagnostics.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$settings` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/settings.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/settings.class.php)[[1654](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/settings.class.php#L1654-L1772)]<br>

<hr>

#### `mailster_do_placeholder`

###### **Filters the replaced content**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->content` | `` | 

Source: [./classes/placeholder.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php)[[621](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php#L621-L626)]<br>

<hr>

#### `mailster_share_button_{$service}`

###### **Builds an HTML share button for a social service.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$content` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/placeholder.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php)[[662](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php#L662-L695)]<br>#### `mailster_prepare_content`

###### **Prepares HTML content for sending by applying Mailster content filters.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$content` | `string` | HTML content.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[1102](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L1102-L1137)]<br>#### `mailster_privacy_content`

###### **Builds suggested privacy policy HTML based on current Mailster settings.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$content` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3.7` | 

Source: [./classes/privacy.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/privacy.class.php)[[41](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/privacy.class.php#L41-L118)]<br>

<hr>

#### `mailster_image_placeholder`

###### **Replaces mailster_image_placeholder URLs with real image markup.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$query['tag']` | `` | 
`$width` | `` | 
`$height` | `` | 
`$crop` | `` | 
`$original` | `` | 
`$this->campaignID` | `` | 
`$this->subscriberID` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3.12` | 

Source: [./classes/placeholder.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php)[[1000](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php#L1000-L1097)]<br>#### `mailster_replace_image`

###### **Replaces mailster_image_placeholder URLs with real image markup.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$replace_to` | `` | 
`$search` | `` | 
`$this->campaignID` | `` | 
`$this->subscriberID` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3.12` | 

Source: [./classes/placeholder.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php)[[1000](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php#L1000-L1193)]<br>#### `mailster_replace_{$tag}`

###### **Replaces static placeholders, custom tags, and fallbacks.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$replace` | `` | 
`$option` | `` | 
`$fallback` | `` | 
`$this->campaignID` | `` | 
`$this->subscriberID` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3.12` | 

Source: [./classes/placeholder.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php)[[1336](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php#L1336-L1429)]<br>#### `mailster_replace_{$post_type}_{$what}`

###### **Resolves a dynamic post property tag to its replacement string.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$replace_to` | `` | 
`$post` | `\WP_Post|object|\WP_Error` | Post-like object.
`$extra` | `` | 
`$this->campaignID` | `` | 
`$this->subscriberID` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/placeholder.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php)[[1444](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php#L1444-L1658)]<br>

<hr>

#### `mailster_get_post_{$post_type}`

###### **Replaces dynamic post-type tags and tweet tags in the content.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$post` | `` | 
`$post_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/placeholder.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php)[[1206](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php#L1206-L1250)]<br>

<hr>

#### `mailster_excerpt_length`

###### **Replaces dynamic post-type tags and tweet tags in the content.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`null` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/placeholder.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php)[[1206](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php#L1206-L1269)]<br>#### `mailster_create_image_unsplash_args`

###### **Returns HTML list markup of posts or media for the campaign post selector.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`array()` | `` | 
`$post_id` | `` | 
`$post->urls->raw` | `` | 
`$post->width` | `` | 
`$post->height` | `` | 
`null` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/ajax.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php)[[1699](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php#L1699-L1852)]<br>#### `mailster_excerpt_length`

###### **Returns placeholder pattern data for a single selected post in the campaign editor.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`null` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/ajax.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php)[[1954](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php#L1954-L1971)]<br>#### `mailster_excerpt_length`

###### **Returns the latest matching post for dynamic campaign content.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`null` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[906](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L906-L1035)]<br>#### `mailster_get_ip`

###### **Detect the client IP address from server variables.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`null` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./includes/functions.php](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php)[[620](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php#L620-L629)]<br>#### `mailster_get_rate_limit_ip`

###### **Return the client IP for rate limiting and anti-flood checks.**

Defaults to REMOTE_ADDR so spoofed X-Forwarded-For headers cannot bypass limits.<br />
Sites behind a trusted reverse proxy may override via the mailster_get_rate_limit_ip filter.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`null` | `` | 

**Changelog**

Version | Description
------- | -----------
`4.1.19` | 

Source: [./includes/functions.php](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php)[[649](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php#L649-L661)]<br>#### `mailster_get_user_client`

###### **Parse and return the visitor user agent client info.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`null` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./includes/functions.php](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php)[[764](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php#L764-L774)]<br>

<hr>

#### `mailster_preview_text_fix`

###### **Adds invisible characters after the preheader text also known as "preview text hack"
Read more here: https://www.litmus.com/blog?p=4367
Updated in Sept. 2023 to use the new invisible characters**

Defaults:<br />
`true`

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`true` | `` | 

Source: [./classes/placeholder.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php)[[1378](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php#L1378-L1388)]<br>#### `mailster_inline_css`

###### **Builds and sends the notification email for a subscriber and options.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`true` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php)[[528](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php#L528-L667)]<br>#### `mailster_inline_css`

###### **Rewrites wp_mail args to use the Mailster system notification template.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`true` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[2773](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L2773-L2879)]<br>

<hr>

#### `mailster_verify_tag`

###### **Inserts or updates a tag row and optionally assigns subscribers.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$entry` | `array|object` | Tag fields (ID, name, added, updated).

**Changelog**

Version | Description
------- | -----------
`3.0` | 

Source: [./classes/tags.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tags.class.php)[[41](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tags.class.php#L41-L68)]<br>#### `mailster_verify_list`

###### **Inserts or updates a list row and optionally assigns subscribers.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$entry` | `array|object` | List fields including optional ID.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php)[[334](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php#L334-L369)]<br>

<hr>

#### `mailster_tag_get_sql`

###### **Loads tags by ID, or all tags, optionally with subscriber counts.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$sql` | `` | 
`null` | `` | 
`$statuses` | `` | 
`$counts` | `bool` | (optional) Include subscriber count column.

**Changelog**

Version | Description
------- | -----------
`3.0` | 

Source: [./classes/tags.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tags.class.php)[[542](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tags.class.php#L542-L578)]<br>#### `mailster_tag_get_sql`

###### **Loads tags by ID, or all tags, optionally with subscriber counts.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$sql` | `` | 
`$id` | `int|int[]|null` | (optional) Tag ID(s); null for all.
`$statuses` | `` | 
`$counts` | `bool` | (optional) Include subscriber count column.

**Changelog**

Version | Description
------- | -----------
`3.0` | 

Source: [./classes/tags.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tags.class.php)[[542](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tags.class.php#L542-L588)]<br>#### `mailster_tag_get_sql`

###### **Loads tags by ID, or all tags, optionally with subscriber counts.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$sql` | `` | 
`$ids` | `` | 
`$statuses` | `` | 
`$counts` | `bool` | (optional) Include subscriber count column.

**Changelog**

Version | Description
------- | -----------
`3.0` | 

Source: [./classes/tags.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tags.class.php)[[542](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tags.class.php#L542-L601)]<br>#### `mailster_list_get_sql`

###### **Fetches one or more lists, optionally with subscriber counts.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$sql` | `` | 
`null` | `` | 
`$statuses` | `` | 
`$counts` | `bool` | Include subscriber count column. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php)[[1004](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php#L1004-L1044)]<br>#### `mailster_list_get_sql`

###### **Fetches one or more lists, optionally with subscriber counts.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$sql` | `` | 
`$id` | `int|array|null` | List id(s), or null for all. (optional).
`$statuses` | `` | 
`$counts` | `bool` | Include subscriber count column. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php)[[1004](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php#L1004-L1060)]<br>#### `mailster_list_get_sql`

###### **Fetches one or more lists, optionally with subscriber counts.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$sql` | `` | 
`$ids` | `` | 
`$statuses` | `` | 
`$counts` | `bool` | Include subscriber count column. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php)[[1004](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php#L1004-L1081)]<br>

<hr>

#### `mailster_get_template_replace`

###### **Loads a campaign template file into the editor and prints the rendered HTML.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$replace` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/ajax.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php)[[336](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php#L336-L418)]<br>

<hr>

#### `mailster_send_test_subject`

###### **Sends a campaign test email to the requested recipients and returns status JSON.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subject` | `` | 
`$receivers` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/ajax.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php)[[809](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php#L809-L871)]<br>

<hr>

#### `mailster_inline_css`

###### **Sends a campaign test email to the requested recipients and returns status JSON.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`true` | `` | 
`$ID` | `` | 
`$subscriber ? $subscriber->ID : null` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/ajax.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php)[[809](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php#L809-L1009)]<br>

<hr>

#### `mailster_auto_tag`

###### **Builds auto-post placeholder tags for a post type and module options.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$pattern` | `` | 
`$post_type` | `` | 
`$options` | `` | 
`$post` | `` | 
`$modulename` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/ajax.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php)[[2034](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php#L2034-L2107)]<br>

<hr>

#### `mailster_dkim_record`

###### **Looks up DKIM DNS records for the configured DKIM selector and domain.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`'k=rsa; p=' . $pubkey` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3.16` | 

Source: [./classes/ajax.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php)[[2712](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php#L2712-L2730)]<br>

<hr>

#### `mailster_workflow_actions`

###### **Returns available workflow action definitions for the editor.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$actions` | `` | 

**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php)[[92](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php#L92-L146)]<br>

<hr>

#### `mailster_workflow_triggers`

###### **Returns available workflow trigger definitions for the editor.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$triggers` | `` | 

**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php)[[151](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php#L151-L237)]<br>

<hr>

#### `mailster_workflow_limit`

###### **Filters the limit of subscribers per workflow run.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`10000` | `` | 

Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php)[[800](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php#L800-L805)]<br>

<hr>

#### `mailster_workflow_runtime`

###### **Filters the max runtime of a workflow.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`15` | `` | 

Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php)[[807](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php#L807-L812)]<br>

<hr>

#### `mailster_automations_allowed_block_types`

###### **Restricts the workflow editor to Mailster workflow blocks.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$types` | `` | 

**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php)[[1670](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php#L1670-L1693)]<br>

<hr>

#### `mailster_rewrite_rules`

###### **Filters Mailster specific rewrite rules**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$rules` | `array` | rewrite rules as assoc array

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php)[[92](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php#L92-L97)]<br>

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

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php)[[380](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php#L380-L388)]<br>#### `mailster_redirect_to`

###### **Filters the redirection target after clicking a link in a campaign**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$redirect_to` | `string` | The redirect link
`$campaign_id` | `int` | Form The ID of the campaign
`$subscriber_id` | `int` | Form The ID of the subscriber
`$campaign_index` | `int` | The index of the link

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php)[[509](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php#L509-L517)]<br>

<hr>

#### `mailster_confirm_target`

###### **Filters the redirection target after clicking a link in a campaign**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$target` | `string` | The redirect link
`$subscriber_id` | `int` | The ID of the subscriber

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php)[[747](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php#L747-L753)]<br>#### `mailster_get_random_post_args`

###### **Returns a pseudo-random post for dynamic campaign content.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$args` | `array` | Extra get_posts args.
`$identifier` | `int` | Seed identifier.
`$post_type` | `string` | Post type.
`$term_ids` | `array` | Taxonomy term ID groups.
`$campaign_id` | `int` | Campaign ID.
`$subscriber_id` | `int|null` | Optional subscriber ID.

**Changelog**

Version | Description
------- | -----------
`2.4` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[830](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L830-L848)]<br>#### `mailster_allow_random_post_duplicates`

###### **Returns a pseudo-random post for dynamic campaign content.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`false` | `` | 
`$post_type` | `string` | Post type.
`$term_ids` | `array` | Taxonomy term ID groups.
`$args` | `array` | Extra get_posts args.
`$campaign_id` | `int` | Campaign ID.
`$subscriber_id` | `int|null` | Optional subscriber ID.

**Changelog**

Version | Description
------- | -----------
`2.4` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[830](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L830-L890)]<br>#### `mailster_pre_get_last_post_args`

###### **Returns the latest matching post for dynamic campaign content.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$args` | `array` | Extra query args.
`$offset` | `int` | Post offset.
`$post_type` | `string` | Post type or rss.
`$term_ids` | `array` | Taxonomy term ID groups.
`$campaign_id` | `int|null` | Optional campaign ID.
`$subscriber_id` | `int|null` | Optional subscriber ID.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[906](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L906-L923)]<br>#### `mailster_get_last_post_{$post_type}`

###### **Returns the latest matching post for dynamic campaign content.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`null` | `` | 
`$args` | `array` | Extra query args.
`$offset` | `int` | Post offset.
`$term_ids` | `array` | Taxonomy term ID groups.
`$campaign_id` | `int|null` | Optional campaign ID.
`$subscriber_id` | `int|null` | Optional subscriber ID.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[906](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L906-L932)]<br>#### `mailster_get_last_post_args`

###### **Returns the latest matching post for dynamic campaign content.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$args` | `array` | Extra query args.
`$offset` | `int` | Post offset.
`$post_type` | `string` | Post type or rss.
`$term_ids` | `array` | Taxonomy term ID groups.
`$campaign_id` | `int|null` | Optional campaign ID.
`$subscriber_id` | `int|null` | Optional subscriber ID.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[906](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L906-L1020)]<br>

<hr>

#### `mailster_cookie_time`

###### **Filters the lifetime of the Mailster cookie.**

Default is 3600 seconds ( 1 Minute )

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$timeout` | `int` | timeout in seconds

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php)[[1198](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php#L1198-L1205)]<br>

<hr>

#### `mailster_editor_tags`

###### **Modify displayed tags in the editbar**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$tags` | `array` | available tags

Source: [./classes/tinymce.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tinymce.class.php)[[151](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tinymce.class.php#L151-L156)]<br>

<hr>

#### `mailster_lists_prepare_items_sql`

###### **Queries and prepares list rows for the current list table request.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$sql` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/lists.table.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.table.class.php)[[280](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.table.class.php#L280-L386)]<br>#### `mailster_campaign_get_subscribers_by_list_sql`

###### **Builds and executes a subscriber query from the given arguments.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$sql` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/subscriber.query.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php)[[239](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php#L239-L1192)]<br>

<hr>

#### `mailster_updatecenter_endpoint`

###### **Requests Freemius migration data and activates the migrated license.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`'https://update.mailster.co/'` | `` | 

**Changelog**

Version | Description
------- | -----------
`3.3.0` | 

Source: [./classes/convert.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/convert.class.php)[[118](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/convert.class.php#L118-L139)]<br>#### `mailster_updatecenter_endpoint`

###### **Fetches license health data and migrates to Freemius when needed.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`'https://update.mailster.co/'` | `` | 

**Changelog**

Version | Description
------- | -----------
`3.3.13` | 

Source: [./classes/health.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/health.class.php)[[63](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/health.class.php#L63-L84)]<br>

<hr>

#### `mailster_conditions_autocomplete_data`

###### **Loads distinct field values for condition autocomplete suggestions.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$data` | `` | 
`$field` | `string` | Condition field key.
`$search` | `string|null` | Optional LIKE search term. (optional).

**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[304](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L304-L374)]<br>

<hr>

#### `mailster_conditions_type_custom_fields`

###### **Returns cached custom field labels including core identity fields.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_custom_fields` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[399](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L399-L420)]<br>

<hr>

#### `mailster_conditions_type_custom_date_fields`

###### **Returns cached custom date field keys.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_custom_date_fields` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[426](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L426-L436)]<br>

<hr>

#### `mailster_conditions_type_fields`

###### **Returns cached core subscriber field labels.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_fields` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[443](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L443-L465)]<br>

<hr>

#### `mailster_conditions_type_time_fields`

###### **Returns field keys that use date/time operators.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_time_fields` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[471](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L471-L482)]<br>

<hr>

#### `mailster_conditions_type_meta_fields`

###### **Returns cached subscriber meta field labels.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_meta_fields` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[489](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L489-L507)]<br>

<hr>

#### `mailster_conditions_type_wp_user_meta`

###### **Returns cached WordPress user meta labels for conditions.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_wp_user_meta` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[595](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L595-L618)]<br>

<hr>

#### `mailster_conditions_type_campaign_related`

###### **Returns campaign engagement condition labels.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_campaign_related` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[624](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L624-L644)]<br>

<hr>

#### `mailster_conditions_type_list_related`

###### **Returns list membership condition labels.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_list_related` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[650](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L650-L663)]<br>

<hr>

#### `mailster_conditions_type_tag_related`

###### **Returns tag condition labels (including deprecated id-based keys).**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_tag_related` | `` | 

**Changelog**

Version | Description
------- | -----------
`3.0` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[669](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L669-L684)]<br>

<hr>

#### `mailster_conditions_type_all_operators`

###### **Returns grouped operators for the condition UI.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_all_operators` | `` | 

**Changelog**

Version | Description
------- | -----------
`3.2.5` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[690](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L690-L710)]<br>

<hr>

#### `mailster_conditions_type_all_value_fields`

###### **Returns known value-field type identifiers.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_all_value_fields` | `` | 

**Changelog**

Version | Description
------- | -----------
`3.2.5` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[716](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L716-L741)]<br>

<hr>

#### `mailster_conditions_type_operators`

###### **Returns general comparison operators.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_operators` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[747](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L747-L770)]<br>

<hr>

#### `mailster_conditions_type_simple_operators`

###### **Returns numeric/simple comparison operators.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_simple_operators` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[776](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L776-L793)]<br>

<hr>

#### `mailster_conditions_type_string_operators`

###### **Returns string comparison operators.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_string_operators` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[799](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L799-L818)]<br>

<hr>

#### `mailster_conditions_type_bool_operators`

###### **Returns boolean comparison operators.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_bool_operators` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[824](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L824-L837)]<br>

<hr>

#### `mailster_conditions_type_date_operators`

###### **Returns absolute date comparison operators.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_date_operators` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[843](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L843-L860)]<br>

<hr>

#### `mailster_conditions_type_relative_date_operators`

###### **Returns relative date comparison operators.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_relative_date_operators` | `` | 

**Changelog**

Version | Description
------- | -----------
`3.1` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[866](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L866-L879)]<br>

<hr>

#### `mailster_conditions_type_special_campaigns`

###### **Returns aggregate campaign option labels.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->_special_campaigns` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/conditions.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php)[[885](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/conditions.class.php#L885-L903)]<br>

<hr>

#### `mailster_pre_create_image`

###### **Resizes or crops an attachment/URL image and returns dimensions and URL.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`null` | `` | 
`$attach_id` | `int|string|null` | Attachment ID or Unsplash id. (optional).
`$img_url` | `string|null` | Image URL or local path. (optional).
`$width` | `int|null` | Target width. (optional).
`$height` | `int|null` | Target height. (optional).
`$crop` | `bool` | Whether to crop. (optional).
`$original` | `bool` | Prefer the original file when possible. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[11](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L11-L28)]<br>#### `mailster_get_bounce_message`

###### **Returns a human-readable message for a bounce status code.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`null` | `` | 
`$status` | `string` | Bounce status code.
`$original` | `string|null` | Fallback/original message. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[1018](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L1018-L1029)]<br>#### `mailster_get_unsubscribe_message`

###### **Returns a human-readable message for an unsubscribe status code.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`null` | `` | 
`$status` | `string` | Unsubscribe status code.
`$original` | `string|null` | Fallback/original message. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2.9` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[1057](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L1057-L1068)]<br>

<hr>

#### `mailster_create_image`

###### **Resizes or crops an attachment/URL image and returns dimensions and URL.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`array('id' => $attach_id, 'url' => $img_url, 'width' => $width, 'height' => $height, 'asp' => $width / $height)` | `` | 
`$attach_id` | `int|string|null` | Attachment ID or Unsplash id. (optional).
`$img_url` | `string|null` | Image URL or local path. (optional).
`$width` | `int|null` | Target width. (optional).
`$height` | `int|null` | Target height. (optional).
`$crop` | `bool` | Whether to crop. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[11](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L11-L90)]<br>#### `mailster_create_image_unsplash_args`

###### **Resizes or crops an attachment/URL image and returns dimensions and URL.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`array()` | `` | 
`$attach_id` | `int|string|null` | Attachment ID or Unsplash id. (optional).
`$img_url` | `string|null` | Image URL or local path. (optional).
`$width` | `int|null` | Target width. (optional).
`$height` | `int|null` | Target height. (optional).
`$crop` | `bool` | Whether to crop. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[11](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L11-L103)]<br>#### `mailster_create_image`

###### **Resizes or crops an attachment/URL image and returns dimensions and URL.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`array('id' => $attach_id, 'url' => $img_url, 'width' => $width, 'height' => $height, 'asp' => $asp)` | `` | 
`$attach_id` | `int|string|null` | Attachment ID or Unsplash id. (optional).
`$img_url` | `string|null` | Image URL or local path. (optional).
`$width` | `int|null` | Target width. (optional).
`$height` | `int|null` | Target height. (optional).
`$crop` | `bool` | Whether to crop. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[11](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L11-L138)]<br>#### `mailster_create_image`

###### **Resizes or crops an attachment/URL image and returns dimensions and URL.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`array('id' => $attach_id, 'url' => $new_img, 'width' => $new_img_size[0], 'height' => $new_img_size[1], 'asp' => $new_img_size[1] ? $new_img_size[0] / $new_img_size[1] : null)` | `` | 
`$attach_id` | `int|string|null` | Attachment ID or Unsplash id. (optional).
`$img_url` | `string|null` | Image URL or local path. (optional).
`$width` | `int|null` | Target width. (optional).
`$height` | `int|null` | Target height. (optional).
`$crop` | `bool` | Whether to crop. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[11](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L11-L230)]<br>

<hr>

#### `mailster_get_social_links`

###### **Returns social profile URL templates, optionally filtered to those with a username.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$links` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[430](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L430-L480)]<br>

<hr>

#### `mailster_using_permalinks`

###### **Whether the site is using pretty permalinks.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`is_object($wp_rewrite) && $wp_rewrite->using_permalinks()` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[681](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L681-L690)]<br>

<hr>

#### `mailster_dateformat`

###### **Returns the site date format string from WordPress settings.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$format` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3.7` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[854](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L854-L865)]<br>#### `mailster_timeformat`

###### **Returns the site time format string from WordPress settings.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$format` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3.7` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[868](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L868-L879)]<br>

<hr>

#### `mailster_strip_shortcode_tags`

###### **Strips or preserves shortcodes in content according to Mailster rules.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`array_keys($shortcode_tags)` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.4.13` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[1140](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L1140-L1159)]<br>

<hr>

#### `mailster_handle_shortcodes`

###### **Strips or preserves shortcodes in content according to Mailster rules.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$content` | `` | 
`$org_content` | `string` | Original content with shortcodes.

**Changelog**

Version | Description
------- | -----------
`2.4.13` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[1140](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L1140-L1169)]<br>#### `mailster_sanitize_content`

###### **Sanitizes campaign HTML for sending, stripping unsafe markup.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$content` | `string` | Raw HTML content.
`$org_content` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[1071](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L1071-L1197)]<br>

<hr>

#### `mailster_post_types`

###### **Returns post types available for dynamic content, minus exclusions.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$post_types` | `` | 
`$output` | `string` | get_post_types() output type. (optional).

**Changelog**

Version | Description
------- | -----------
`2.4` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[1735](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L1735-L1753)]<br>#### `mailster_dynamic_post_types`

###### **Returns post types for dynamic modules, filterable via mailster_dynamic_post_types.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->get_post_types($public_only, $output, $exclude)` | `` | 
`$output` | `string` | get_post_types() output type. (optional).

**Changelog**

Version | Description
------- | -----------
`2.4` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[1756](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L1756-L1768)]<br>

<hr>

#### `mailster_feed_cache_duration`

###### **Fetches and caches an RSS/Atom feed, optionally returning a single item.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`360` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.4` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[1771](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L1771-L1793)]<br>

<hr>

#### `mailster_feed_max_items`

###### **Fetches and caches an RSS/Atom feed, optionally returning a single item.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`100` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.4` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[1771](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L1771-L1849)]<br>

<hr>

#### `mailster_pre_get_excerpt`

###### **Builds a text excerpt of a given length with an optional more suffix.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`null` | `` | 
`$org_string` | `string` | Source text.
`$length` | `int|null` | Max length. (optional).
`$more` | `string|null` | More suffix. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[2091](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L2091-L2107)]<br>#### `mailster_get_excerpt`

###### **Builds a text excerpt of a given length with an optional more suffix.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$excerpt` | `` | 
`$org_string` | `string` | Source text.
`$length` | `int|null` | Max length. (optional).
`$more` | `string|null` | More suffix. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[2091](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L2091-L2139)]<br>

<hr>

#### `mailster_plain_text`

###### **Converts HTML to plain text, optionally listing links.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`null` | `` | 
`$html` | `string` | HTML content.
`$linksonly` | `bool` | Append collected URLs. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2.5` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[2144](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L2144-L2156)]<br>

<hr>

#### `mailster_subscriber_notification_subscriber_limit`

###### **Renders a delayed digest of recent new subscribers, or delegates to the single template.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`7` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php)[[1078](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php#L1078-L1092)]<br>#### `mailster_subscriber_unsubscribe_notification_subscriber_limit`

###### **Renders a delayed digest of recent unsubscriptions, or delegates to the single template.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`7` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php)[[1472](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php#L1472-L1486)]<br>

<hr>

#### `mailster_precheck_mail`

###### **Sends a health-check test email via the notification system.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`'mailster-' . $precheck_id . '@precheck.email'` | `` | 
`$precheck_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`3.3.13` | 

Source: [./classes/health.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/health.class.php)[[130](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/health.class.php#L130-L140)]<br>

<hr>

#### `mailster_time_check_value`

###### **Seconds to prevent forms being submitted**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`4` | `` | 

Source: [./classes/rest-controller/rest.form.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/rest-controller/rest.form.class.php)[[200](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/rest-controller/rest.form.class.php#L200-L205)]<br>

<hr>

#### `mailster_block_form_field_errors`

###### **Allow third parties to hook into the form submission errors**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$fields_errors` | `array` | all current error
`$entry` | `array` | the collected user data
`$request` | `object` | the request

Source: [./classes/rest-controller/rest.form.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/rest-controller/rest.form.class.php)[[211](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/rest-controller/rest.form.class.php#L211-L218)]<br>

<hr>

#### `mailster_forms_allowed_block_types`

###### **Restricts the form editor to core and Mailster form blocks.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`array_values($types)` | `` | 

**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/block-forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/block-forms.class.php)[[1530](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/block-forms.class.php#L1530-L1561)]<br>

<hr>

#### `mailster_block_form`

###### **Server-side render callback for the mailster/form block.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$output` | `` | 
`$form->ID` | `` | 
`$form_args` | `` | 

**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/block-forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/block-forms.class.php)[[1844](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/block-forms.class.php#L1844-L2228)]<br>

<hr>

#### `mailster_freemius_args`

###### **Initializes and returns the Freemius SDK instance.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`array('id' => 12184, 'slug' => 'mailster', 'public_key' => 'pk_1efa30140fc34f21e5b89959bb877', 'is_premium' => true, 'is_premium_only' => true, 'has_addons' => false, 'has_paid_plans' => true, 'is_org_compliant' => false, 'trial' => array('days' => 14, 'is_require_payment' => false), 'menu' => array('slug' => 'edit.php?post_type=newsletter', 'first-path' => 'admin.php?page=mailster_dashboard', 'contact' => false, 'support' => false, 'pricing' => false, 'affiliation' => false, 'account' => true))` | `` | 

**Changelog**

Version | Description
------- | -----------
`3.3.0` | 

Source: [./classes/license.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/license.class.php)[[50](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/license.class.php#L50-L88)]<br>

<hr>

#### `mailster_subscriber_query_args`

###### **Builds and executes a subscriber query from the given arguments.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->args` | `` | 
`$campaign_id` | `int|null` | (optional) Campaign ID for action joins and caching.

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/subscriber.query.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php)[[239](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php#L239-L535)]<br>#### `mailster_subscriber_query_sql_joins`

###### **Builds and executes a subscriber query from the given arguments.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$joins` | `` | 
`$this->args` | `` | 
`$campaign_id` | `int|null` | (optional) Campaign ID for action joins and caching.

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/subscriber.query.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php)[[239](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php#L239-L1143)]<br>#### `mailster_subscriber_query_sql_wheres`

###### **Builds and executes a subscriber query from the given arguments.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$wheres` | `` | 
`$this->args` | `` | 
`$campaign_id` | `int|null` | (optional) Campaign ID for action joins and caching.

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/subscriber.query.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php)[[239](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php#L239-L1149)]<br>#### `mailster_subscriber_query_sql_groupby`

###### **Builds and executes a subscriber query from the given arguments.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->args['groupby']` | `` | 
`$this->args` | `` | 
`$campaign_id` | `int|null` | (optional) Campaign ID for action joins and caching.

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/subscriber.query.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php)[[239](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php#L239-L1155)]<br>#### `mailster_subscriber_query_sql_havings`

###### **Builds and executes a subscriber query from the given arguments.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this->args['having']` | `` | 
`$this->args` | `` | 
`$campaign_id` | `int|null` | (optional) Campaign ID for action joins and caching.

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/subscriber.query.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php)[[239](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php#L239-L1161)]<br>#### `mailster_subscriber_query_sql_orders`

###### **Builds and executes a subscriber query from the given arguments.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$orders` | `` | 
`$this->args` | `` | 
`$campaign_id` | `int|null` | (optional) Campaign ID for action joins and caching.

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/subscriber.query.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php)[[239](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php#L239-L1167)]<br>#### `mailster_subscriber_query_sql`

###### **Builds and executes a subscriber query from the given arguments.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$sql` | `` | 
`$this->args` | `` | 
`$campaign_id` | `int|null` | (optional) Campaign ID for action joins and caching.

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/subscriber.query.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php)[[239](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscriber.query.class.php#L239-L1194)]<br>#### `mailster_unsubscribe_link`

###### **Builds an unsubscribe URL for a campaign and subscriber hash.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$unsubscribe_homepage` | `` | 
`$campaign_id` | `int|string|null` | Optional campaign ID.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[545](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L545-L582)]<br>

<hr>

#### `mailster_classes`

###### **Loads subsystem classes, applies the mailster_classes filter, and initializes hooks.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`array('settings' => new MailsterSettings(), 'convert' => new MailsterConvert(), 'api' => new MailsterApi(), 'translations' => new MailsterTranslations(), 'logs' => new MailsterLogs(), 'campaigns' => new MailsterCampaigns(), 'subscribers' => new MailsterSubscribers(), 'automations' => new MailsterAutomations(), 'triggers' => new MailsterTrigger(), 'lists' => new MailsterLists(), 'tags' => new MailsterTags(), 'block-forms' => new MailsterBlockForms(), 'forms' => new MailsterForms(), 'precheck' => new MailsterPrecheck(), 'manage' => new MailsterManage(), 'templates' => new MailsterTemplates(), 'addons' => new MailsterAddons(), 'frontpage' => new MailsterFrontpage(), 'statistics' => new MailsterStatistics(), 'ajax' => new MailsterAjax(), 'tinymce' => new MailsterTinymce(), 'cron' => new MailsterCron(), 'queue' => new MailsterQueue(), 'actions' => new MailsterActions(), 'bounce' => new MailsterBounce(), 'dashboard' => new MailsterDashboard(), 'update' => new MailsterUpdate(), 'upgrade' => new MailsterUpgrade(), 'helpmenu' => new MailsterHelpmenu(), 'geo' => new MailsterGeo(), 'privacy' => new MailsterPrivacy(), 'health' => new MailsterHealth(), 'security' => new MailsterSecurity(), 'export' => new MailsterExport(), 'notices' => new MailsterNotices(), 'empty' => new MailsterEmpty())` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[37](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L37-L124)]<br>

<hr>

#### `mailster_encode_link`

###### **Base64url-encodes a destination URL for tracking.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`rtrim(strtr(base64_encode($link), '+/', '-_'), '=')` | `` | 
`$link` | `string` | Destination URL.

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[806](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L806-L815)]<br>

<hr>

#### `mailster_decode_link`

###### **Decodes a base64url-encoded tracking link.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`base64_decode(strtr($encoded_link, '-_', '+/'))` | `` | 
`$encoded_link` | `string` | Encoded link token.

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[818](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L818-L827)]<br>

<hr>

#### `mailster_get_random_post_seed`

###### **Returns a pseudo-random post for dynamic campaign content.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`0` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.4` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[830](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L830-L855)]<br>

<hr>

#### `mailster_allowed_script_domains`

###### **Sanitizes campaign HTML for sending, stripping unsafe markup.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`array('cdn.ampproject.org')` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[1071](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L1071-L1127)]<br>

<hr>

#### `mailster_allowed_script_types`

###### **Sanitizes campaign HTML for sending, stripping unsafe markup.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`array('application/ld+json')` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[1071](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L1071-L1128)]<br>

<hr>

#### `mailster_allowed_tags`

###### **Sanitizes campaign HTML for sending, stripping unsafe markup.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$allowed_tags` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[1071](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L1071-L1157)]<br>

<hr>

#### `mailster_localize_script`

###### **Prints localized mailster_l10n strings for admin scripts.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`array()` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.4.10` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[1531](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L1531-L1539)]<br>

<hr>

#### `mailster_table_structure`

###### **Returns CREATE TABLE SQL statements for Mailster tables.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$table_structure` | `` | 
`$collate` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[2182](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L2182-L2510)]<br>

<hr>

#### `mailster_wp_mail_template`

###### **Rewrites wp_mail args to use the Mailster system notification template.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$template` | `` | 
`$caller` | `` | 
`$current_filter` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[2773](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L2773-L2818)]<br>#### `mailster_wp_mail_template_file`

###### **Rewrites wp_mail args to use the Mailster system notification template.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$file` | `` | 
`$caller` | `` | 
`$current_filter` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[2773](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L2773-L2827)]<br>#### `mailster_send_replace`

###### **Rewrites wp_mail args to use the Mailster system notification template.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$replace` | `` | 
`$caller` | `` | 
`$current_filter` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[2773](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L2773-L2844)]<br>#### `mailster_send_message`

###### **Rewrites wp_mail args to use the Mailster system notification template.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$args['message']` | `` | 
`$caller` | `` | 
`$current_filter` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[2773](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L2773-L2845)]<br>#### `mailster_send_subject`

###### **Rewrites wp_mail args to use the Mailster system notification template.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$args['subject']` | `` | 
`$caller` | `` | 
`$current_filter` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[2773](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L2773-L2846)]<br>#### `mailster_send_headline`

###### **Rewrites wp_mail args to use the Mailster system notification template.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$args['subject']` | `` | 
`$caller` | `` | 
`$current_filter` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[2773](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L2773-L2847)]<br>#### `mailster_wp_mail_template`

###### **Sends mail through Mailster using the notification template system.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$template` | `string|null` | Optional template slug.
`$caller` | `` | 
`$current_filter` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[2917](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L2917-L2997)]<br>#### `mailster_wp_mail_template_file`

###### **Sends mail through Mailster using the notification template system.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$file` | `string|null` | Optional notification template file.
`$caller` | `` | 
`$current_filter` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[2917](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L2917-L3004)]<br>

<hr>

#### `mailster_send_replace`

###### **Sends mail through Mailster using the notification template system.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`array('notification' => '')` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[2917](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L2917-L3042)]<br>

<hr>

#### `mailster_send_message`

###### **Sends mail through Mailster using the notification template system.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$message` | `string` | Email body.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[2917](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L2917-L3043)]<br>

<hr>

#### `mailster_send_headline`

###### **Sends mail through Mailster using the notification template system.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subject` | `string` | Email subject.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[2917](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L2917-L3044)]<br>

<hr>

#### `mailster_form_url`

###### **Builds a public form URL with query args, filterable via mailster_form_url.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`add_query_arg($args, $endpoint)` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[705](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L705-L720)]<br>

<hr>

#### `mailster_autoresponder_grace_period`

###### **Filter the grace period from campaigns to decide the time when user no longer get the campaign.**

Default: 604800 (one week).

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$grace_period` | `int|false` | The grace period in seconds. Set to false to disable.
`$campaign` | `\WP_Post` | The campaign post object.

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php)[[472](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php#L472-L480)]<br>

<hr>

#### `mailster_autoresponder_hook_args`

###### **Queues autoresponder campaigns driven by subscribe, unsubscribe, follow-up, or RSS.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$query_args` | `` | 
`$campaign->ID` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php)[[416](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php#L416-L520)]<br>#### `mailster_autoresponder_hook_args`

###### **Queues autoresponder campaigns driven by subscribe, unsubscribe, follow-up, or RSS.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$query_args` | `` | 
`$campaign->ID` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php)[[416](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php#L416-L560)]<br>#### `mailster_autoresponder_hook_args`

###### **Queues autoresponder campaigns driven by subscribe, unsubscribe, follow-up, or RSS.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$query_args` | `` | 
`$campaign->ID` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php)[[416](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php#L416-L619)]<br>

<hr>

#### `mailster_unlock_cron`

###### **Processes due queue entries: sends campaign and notification emails for this cron turn.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`false` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php)[[1062](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php#L1062-L1112)]<br>

<hr>

#### `mailster_unsubscribe_link`

###### **Processes due queue entries: sends campaign and notification emails for this cron turn.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`get_page(mailster_option('homepage')) ? get_permalink(mailster_option('homepage')) : get_bloginfo('url')` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php)[[1062](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php#L1062-L1172)]<br>

<hr>

#### `mailster_queue_campaign_subscriber_data`

###### **Processes due queue entries: sends campaign and notification emails for this cron turn.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$data` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php)[[1062](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php#L1062-L1278)]<br>

<hr>

#### `mailster_dep_domains`

###### **Returns disposable email provider domains used for rejection.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$dep_domains` | `` | 

**Changelog**

Version | Description
------- | -----------
`3.0` | 

Source: [./classes/security.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/security.class.php)[[244](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/security.class.php#L244-L255)]<br>

<hr>

#### `mailster_importer`

###### **Instantiates registered importer classes into $integrations.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`array('MailsterImportUpload' => MAILSTER_DIR . 'classes/manage.import.upload.php', 'MailsterImportPaste' => MAILSTER_DIR . 'classes/manage.import.paste.php', 'MailsterImportWordPress' => MAILSTER_DIR . 'classes/manage.import.wordpress.php')` | `` | 

**Changelog**

Version | Description
------- | -----------
`3.1` | 

Source: [./classes/manage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/manage.class.php)[[47](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/manage.class.php#L47-L63)]<br>

<hr>

#### `mailster_export_args`

###### **AJAX: prepares an export job and returns subscriber IDs to process.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$args` | `` | 
`$post_data` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/manage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/manage.class.php)[[962](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/manage.class.php#L962-L998)]<br>#### `mailster_export_heading_{$col}`

###### **AJAX: writes the next chunk of subscriber rows into the export file.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$val` | `` | 
`$post_data` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/manage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/manage.class.php)[[1055](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/manage.class.php#L1055-L1173)]<br>#### `mailster_export_args`

###### **AJAX: writes the next chunk of subscriber rows into the export file.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$args` | `` | 
`$post_data` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/manage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/manage.class.php)[[1055](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/manage.class.php#L1055-L1221)]<br>#### `mailster_export_field_{$key}`

###### **AJAX: writes the next chunk of subscriber rows into the export file.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$val` | `` | 
`$post_data` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/manage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/manage.class.php)[[1055](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/manage.class.php#L1055-L1293)]<br>

<hr>

#### `mailster_cron_url`

###### **Returns the public or AJAX URL used to trigger the Mailster cron endpoint.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`get_home_url(null, 'mailster/' . mailster_option('cron_secret'))` | `` | 
`$alternative` | `bool` | (optional) Use the admin-ajax endpoint instead of the pretty URL.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/cron.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/cron.class.php)[[456](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/cron.class.php#L456-L469)]<br>#### `mailster_cron_url`

###### **Returns the public or AJAX URL used to trigger the Mailster cron endpoint.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`add_query_arg(array('secret' => mailster_option('cron_secret')), MAILSTER_URI . 'cron.php')` | `` | 
`$alternative` | `bool` | (optional) Use the admin-ajax endpoint instead of the pretty URL.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/cron.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/cron.class.php)[[456](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/cron.class.php#L456-L480)]<br>#### `mailster_cron_url`

###### **Returns the public or AJAX URL used to trigger the Mailster cron endpoint.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`add_query_arg(array('action' => 'mailster_cron', 'secret' => mailster_option('cron_secret')), admin_url('admin-ajax.php'))` | `` | 
`$alternative` | `bool` | (optional) Use the admin-ajax endpoint instead of the pretty URL.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/cron.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/cron.class.php)[[456](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/cron.class.php#L456-L494)]<br>

<hr>

#### `mailster_subscriber_errors`

###### **Default subscriber errors where campaigns do not get paused or skipped.**

Defaults:<br />
`SMTP Error: The following recipients failed`<br />
`The following From address failed`<br />
`Invalid address:`<br />
`SMTP Error: Data not accepted`

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$default` | `array` | Default values.

Source: [./classes/mail.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.class.php)[[495](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.class.php#L495-L506)]<br>#### `mailster_server_errors`

###### **Default server errors where campaigns get paused or skipped.**

Defaults:<br />
`Sender address rejected`

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$default` | `array` | Default values.

Source: [./classes/mail.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.class.php)[[511](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.class.php#L511-L519)]<br>#### `mailster_system_errors`

###### **Default system errors where campaigns get paused or skipped.**

Defaults:<br />
`Not in Time Frame`

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$default` | `array` | Default values.

Source: [./classes/mail.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.class.php)[[524](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.class.php#L524-L532)]<br>

<hr>

#### `mailster_mail_set_{$name}`

###### **Magic setter that filters values via mailster_mail_set_{$name}.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$value` | `mixed` | Property value.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mail.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.class.php)[[656](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.class.php#L656-L670)]<br>

<hr>

#### `mailster_inline_css`

###### **Filter to skip inline CSS**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$inline_css` | `bool` | Whenever to enable inline styles or not

Source: [./classes/mail.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.class.php)[[971](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.class.php#L971-L976)]<br>

<hr>

#### `mailster_cron_simple_output`

###### **Filter the output of the cron page.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`(bool) preg_match('/curl|wget/i', $user_agent) || isset($_GET['simple'])` | `` | 

**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./includes/cron.php](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/cron.php)[[40](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/cron.php#L40-L47)]<br>

<hr>

#### `mailster_option`

###### **Retrieve a Mailster option value.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$value` | `` | 
`$option` | `string` | Option.
`$fallback` | `mixed` | Fallback Optional.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./includes/functions.php](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php)[[32](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php#L32-L46)]<br>#### `mailster_option_{$option}`

###### **Retrieve a Mailster option value.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$value` | `` | 
`$fallback` | `mixed` | Fallback Optional.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./includes/functions.php](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php)[[32](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php#L32-L47)]<br>#### `mailster_text`

###### **Retrieve a translatable Mailster text string.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$string` | `` | 
`$option` | `string` | Option.
`$fallback` | `mixed` | Fallback Optional.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./includes/functions.php](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php)[[165](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php#L165-L180)]<br>

<hr>

#### `mailster_update_option_{$option}`

###### **Update one or more Mailster option values.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$value` | `mixed` | Value Optional.
`$temp` | `bool` | Temp Optional.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./includes/functions.php](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php)[[192](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php#L192-L210)]<br>

<hr>

#### `mailster_list_newsletter`

###### **Output or return an HTML list of newsletter archive links.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$output` | `` | 
`$r` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./includes/functions.php](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php)[[500](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/functions.php#L500-L545)]<br>

<hr>

#### `mailster_help_pages`

###### **Help Scout beacon configuration for admin screens.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`array(
    // newsletter edit page.
    'newsletter' => array('tabs' => array(array('title' => 'More')), 'sidebar' => 'sidebar'),
    'newsletter_page_mailster_subscribers' => array('tabs' => array(array('title' => 'More')), 'sidebar' => 'sidebar'),
    'newsletter_page_mailster_lists' => array('tabs' => array(array('title' => 'More')), 'sidebar' => 'sidebar'),
    'newsletter_page_mailster_manage_subscribers' => array('tabs' => array(array('title' => 'More')), 'sidebar' => 'sidebar'),
    'newsletter_page_mailster_dashboard' => array('tabs' => array(array('title' => 'More')), 'sidebar' => 'sidebar'),
)` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./includes/helppages.php](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/helppages.php)[[2](https://github.com/everpress-co/mailster/blob/4.1.22/./includes/helppages.php#L2-L35)]<br>



