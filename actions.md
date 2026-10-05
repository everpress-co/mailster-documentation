# Actions
Mailster provides various hooks and filters you can use to alter the behavior of the plugin or write your own add-ons and extensions. We recommend to read more about hooks on the [official site](https://developer.wordpress.org/plugins/hooks/).

!>  While there are more hooks in the plugin we only list a few here.

<hr>

#### `mailster_update_homepage`

###### **Flushes rewrite rules when the configured newsletter homepage is updated.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$post` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php)[[102](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php#L102-L115)]<br>

<hr>

#### `mailster_click`

###### **Fires if user clicks on a link and tracking is enabled**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `int` | The ID of the subscriber
`$campaign_id` | `int` | Form The ID of the campaign
`$target` | `string` | The target link
`$index` | `int` | The index of the link
`$campaign_index` | `int` | The index of the campaign

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php)[[470](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php#L470-L479)]<br>#### `mailster_open`

###### **Fires if user opens on a campaign and tracking is enabled**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `int` | The ID of the subscriber
`$campaign_id` | `int` | Form The ID of the campaign
`$campaign_index` | `int` | The index of the campaign

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php)[[483](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php#L483-L490)]<br>

<hr>

#### `mailster_homepage_subscribe`

###### **Handles subscribe, unsubscribe, profile, and confirm homepage subpages.**


**Changelog**

Version | Description
------- | -----------
`2.2.8` | 

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php)[[558](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php#L558-L577)]<br>

<hr>

#### `mailster_homepage_unsubscribe`

###### **Handles subscribe, unsubscribe, profile, and confirm homepage subpages.**


**Changelog**

Version | Description
------- | -----------
`2.2.8` | 

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php)[[558](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php#L558-L613)]<br>

<hr>

#### `mailster_homepage_profile`

###### **Handles subscribe, unsubscribe, profile, and confirm homepage subpages.**


**Changelog**

Version | Description
------- | -----------
`2.2.8` | 

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php)[[558](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php#L558-L629)]<br>

<hr>

#### `mailster_homepage_confirm`

###### **Handles subscribe, unsubscribe, profile, and confirm homepage subpages.**


**Changelog**

Version | Description
------- | -----------
`2.2.8` | 

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php)[[558](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php#L558-L652)]<br>

<hr>

#### `mailster_subscriber_subscribed`

###### **Run after the users confirms the subscription**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `int` | The ID of the subscriber

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php)[[729](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php#L729-L734)]<br>#### `mailster_subscriber_save`

###### **Handles create and update submissions on the subscriber edit screen.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php)[[445](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php#L445-L474)]<br>#### `mailster_update_subscriber`

###### **Updates an existing subscriber or creates one when missing.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php)[[1103](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php#L1103-L1292)]<br>#### `mailster_add_subscriber`

###### **Adds a new subscriber, optionally overwriting or merging an existing one.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php)[[1320](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php#L1320-L1387)]<br>#### `mailster_list_unconfirmed`

###### **Clears the list membership `added` timestamp for a subscriber.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$list_id` | `int` | List id.
`$subscriber_id` | `int` | Subscriber id.

**Changelog**

Version | Description
------- | -----------
`2.3.2` | 

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/lists.class.php)[[623](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/lists.class.php#L623-L650)]<br>#### `mailster_list_removed`

###### **Deletes a list–subscriber relationship.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$list_id` | `int` | List id.
`$subscriber_id` | `int` | Subscriber id.

**Changelog**

Version | Description
------- | -----------
`2.2.3` | 

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/lists.class.php)[[789](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/lists.class.php#L789-L813)]<br>

<hr>

#### `mailster_frontpage`

###### **Renders a single newsletter web version with or without the frame chrome.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php)[[817](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php#L817-L839)]<br>

<hr>

#### `mailster_frontpage_frame`

###### **Renders a single newsletter web version with or without the frame chrome.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php)[[817](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/frontpage.class.php#L817-L890)]<br>

<hr>

#### `mailster_check_bounces`

###### **Hourly maintenance: bounce check, resend confirmations, and refresh schedules.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/cron.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/cron.class.php)[[47](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/cron.class.php#L47-L57)]<br>

<hr>

#### `mailster_resend_confirmations`

###### **Hourly maintenance: bounce check, resend confirmations, and refresh schedules.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/cron.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/cron.class.php)[[47](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/cron.class.php#L47-L60)]<br>

<hr>

#### `mailster_update_tag`

###### **Inserts or updates a tag row and optionally assigns subscribers.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$tag_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`3.0` | 

Source: [./classes/tags.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/tags.class.php)[[40](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/tags.class.php#L40-L105)]<br>

<hr>

#### `mailster_tag_added`

###### **Assigns a single tag to a single subscriber.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$tag_id` | `int|string` | Tag ID or name.
`$subscriber_id` | `int` | Subscriber ID.
`$name` | `` | 

**Changelog**

Version | Description
------- | -----------
`3.0` | 

Source: [./classes/tags.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/tags.class.php)[[253](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/tags.class.php#L253-L282)]<br>#### `mailster_tag_removed`

###### **Unassigns a single tag from a single subscriber.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$tag_id` | `int|string` | Tag ID or name.
`$subscriber_id` | `int` | Subscriber ID.
`$name` | `` | 

**Changelog**

Version | Description
------- | -----------
`3.0` | 

Source: [./classes/tags.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/tags.class.php)[[330](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/tags.class.php#L330-L358)]<br>

<hr>

#### `mailster`

###### **Registers core cron, admin, block, and REST hooks.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/mailster.class.php)[[323](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/mailster.class.php#L323-L371)]<br>#### `mailster_initsend`

###### **Configures the mailer transport, DKIM, limits, and error classifiers.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mail.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/mail.class.php)[[411](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/mail.class.php#L411-L466)]<br>#### `mailster_presend`

###### **Runs presend/dosend hooks and returns the Message-ID when sent.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mail.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/mail.class.php)[[988](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/mail.class.php#L988-L1006)]<br>#### `mailster_dosend`

###### **Runs presend/dosend hooks and returns the Message-ID when sent.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mail.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/mail.class.php)[[988](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/mail.class.php#L988-L1012)]<br>

<hr>

#### `mailster_admin_header`

###### **Fires mailster_admin_header on newsletter admin screens.**


**Changelog**

Version | Description
------- | -----------
`3.2.5` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/mailster.class.php)[[1280](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/mailster.class.php#L1280-L1296)]<br>Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/mailster.class.php)[[1538](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/mailster.class.php#L1538-L1550)]<br>Source: [./classes/upgrade.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/upgrade.class.php)[[493](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/upgrade.class.php#L493-L504)]<br>Source: [./classes/health.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/health.class.php)[[46](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/health.class.php#L46-L55)]<br>Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/automation.class.php)[[1571](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/automation.class.php#L1571-L1591)]<br>Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/automation.class.php)[[1596](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/automation.class.php#L1596-L1611)]<br>Source: [./classes/block-forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/block-forms.class.php)[[1436](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/block-forms.class.php#L1436-L1456)]<br>Source: [./classes/block-forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/block-forms.class.php)[[1465](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/block-forms.class.php#L1465-L1480)]<br>

<hr>

#### `mailster_page_beacon_{$screen->id}`

###### **Outputs contextual Helpscout beacon help links for the current screen.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$tab` | `` | 

**Changelog**

Version | Description
------- | -----------
`3.2.5` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/mailster.class.php)[[1338](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/mailster.class.php#L1338-L1398)]<br>

<hr>

#### `mailster_thirdpartystuff`

###### **Hooks third-party cache flush helpers on shutdown.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/mailster.class.php)[[3574](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/mailster.class.php#L3574-L3583)]<br>

<hr>

#### `mailster_add_tag`

###### **Replaces static placeholders, custom tags, and fallbacks.**


**Changelog**

Version | Description
------- | -----------
`2.3.12` | 

Source: [./classes/placeholder.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/placeholder.class.php)[[1330](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/placeholder.class.php#L1330-L1343)]<br>Source: [./classes/tinymce.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/tinymce.class.php)[[71](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/tinymce.class.php#L71-L84)]<br>

<hr>

#### `mailster_precheck_script_styles`

###### **Prints and returns the Precheck editor CSS and JavaScript assets.**


**Changelog**

Version | Description
------- | -----------
`3.0` | 

Source: [./classes/precheck.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/precheck.class.php)[[17](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/precheck.class.php#L17-L37)]<br>

<hr>

#### `mailster_cron`

###### **Redirects incomplete setup or pending DB updates before the dashboard loads.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/dashboard.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/dashboard.class.php)[[74](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/dashboard.class.php#L74-L88)]<br>Source: [./classes/ajax.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/ajax.class.php)[[3409](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/ajax.class.php#L3409-L3472)]<br>

<hr>

#### `mailster_notification_{$template}`

###### **Builds and sends the notification email for a subscriber and options.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber` | `` | 
`$options` | `array` | Send options including template and field overrides.
`$output` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/notification.class.php)[[527](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/notification.class.php#L527-L568)]<br>

<hr>

#### `mailster_freemius_loaded`

###### **Initializes and returns the Freemius SDK instance.**


**Changelog**

Version | Description
------- | -----------
`3.3.0` | 

Source: [./classes/license.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/license.class.php)[[49](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/license.class.php#L49-L92)]<br>

<hr>

#### `mailster_autoresponder_post_published`

###### **Queues autoresponder campaigns driven by subscribe, unsubscribe, follow-up, or RSS.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$campaign->ID` | `` | 
`$new_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/queue.class.php)[[415](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/queue.class.php#L415-L691)]<br>#### `mailster_autoresponder_timebased`

###### **Creates scheduled campaigns from time-based autoresponder parents.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$campaign->ID` | `` | 
`$new_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/queue.class.php)[[711](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/queue.class.php#L711-L851)]<br>#### `mailster_workflow_duplicate`

###### **Creates a draft copy of a workflow, optionally overriding args or meta.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$id` | `int` | Source workflow post ID.
`$new_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`4.1.0` | 

Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/automation.class.php)[[1930](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/automation.class.php#L1930-L1986)]<br>#### `mailster_campaign_duplicate`

###### **Duplicates a campaign with optional post and meta overrides.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$id` | `int` | Source campaign ID.
`$new_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php)[[3184](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php#L3184-L3254)]<br>#### `mailster_autoresponder_post_published`

###### **Evaluates and queues autoresponder campaigns for a published post.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$campaign->ID` | `` | 
`$new_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php)[[5865](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php#L5865-L5970)]<br>#### `mailster_form_duplicate`

###### **Duplicates a form including fields, lists, and tags.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$id` | `int` | Source form ID.
`$new_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php)[[851](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php#L851-L899)]<br>

<hr>

#### `mailster_autoresponder_usertime`

###### **Queues autoresponders based on subscriber custom date fields.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$campaign->ID` | `` | 
`$subscriber_ids` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/queue.class.php)[[872](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/queue.class.php#L872-L1021)]<br>

<hr>

#### `mailster_subscriber_error`

###### **Processes due queue entries: sends campaign and notification emails for this cron turn.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$data->subscriber_id` | `` | 
`$data->campaign_id` | `` | 
`$result->get_error_message()` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/queue.class.php)[[1061](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/queue.class.php#L1061-L1365)]<br>#### `mailster_notification_error`

###### **Processes due queue entries: sends campaign and notification emails for this cron turn.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$data->subscriber_id` | `` | 
`$result->get_error_message()` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/queue.class.php)[[1061](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/queue.class.php#L1061-L1382)]<br>#### `mailster_campaign_error`

###### **Processes due queue entries: sends campaign and notification emails for this cron turn.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$data->subscriber_id` | `` | 
`$data->campaign_id` | `` | 
`$result->get_error_message()` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/queue.class.php)[[1061](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/queue.class.php#L1061-L1403)]<br>#### `mailster_system_error`

###### **Processes due queue entries: sends campaign and notification emails for this cron turn.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$data->subscriber_id` | `` | 
`$data->campaign_id` | `` | 
`$result->get_error_message()` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/queue.class.php)[[1061](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/queue.class.php#L1061-L1409)]<br>

<hr>

#### `mailster_cron_finished`

###### **Processes due queue entries: sends campaign and notification emails for this cron turn.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/queue.class.php)[[1061](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/queue.class.php#L1061-L1498)]<br>

<hr>

#### `mailster_subscriber_save`

###### **Handles create and update submissions on the subscriber edit screen.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber->ID` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php)[[445](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php#L445-L579)]<br>

<hr>

#### `mailster_subscriber_delete`

###### **Handles create and update submissions on the subscriber edit screen.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber->ID` | `` | 
`$subscriber->email` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php)[[445](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php#L445-L601)]<br>#### `mailster_subscriber_delete`

###### **Handles create and update submissions on the subscriber edit screen.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber->ID` | `` | 
`$subscriber->email` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php)[[445](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php#L445-L636)]<br>

<hr>

#### `mailster_add_custom_field`

###### **Inserts a custom field row for a subscriber, optionally updating if it exists.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `int` | Subscriber ID.
`$key` | `string` | Field or meta key.
`$value` | `string|null` | Value to store or filter.

**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php)[[1559](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php#L1559-L1617)]<br>

<hr>

#### `mailster_update_custom_field`

###### **Updates an existing custom field value for a subscriber.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `int` | Subscriber ID.
`$key` | `string` | Field or meta key.
`$value` | `string|null` | Value to store or filter.
`$old_value` | `` | 

**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php)[[1628](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php#L1628-L1679)]<br>#### `mailster_remove_custom_field`

###### **Deletes a custom field row for a subscriber.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `int` | Subscriber ID.
`$key` | `string` | Field or meta key.
`$old_value` | `` | 

**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php)[[1690](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php#L1690-L1718)]<br>

<hr>

#### `mailster_list_unsubscribe`

###### **Unsubscribes a subscriber looked up by an arbitrary field type.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber->ID` | `` | 
`$campaign_id` | `int|null` | Campaign ID.
`$lists` | `` | 
`$status` | `string|null` | Status value or filter.
`$index` | `int|null` | Campaign queue index.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php)[[3249](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php#L3249-L3292)]<br>#### `mailster_unsubscribe`

###### **Unsubscribes a subscriber looked up by an arbitrary field type.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber->ID` | `` | 
`$campaign_id` | `int|null` | Campaign ID.
`$status` | `string|null` | Status value or filter.
`$index` | `int|null` | Campaign queue index.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php)[[3249](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php#L3249-L3312)]<br>#### `mailster_bounce`

###### **Records a hard or soft bounce for a subscriber and campaign.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber->ID` | `` | 
`$campaign_id` | `int` | Campaign ID.
`true` | `` | 
`$status` | `string|null` | Status value or filter.
`$index` | `int|null` | Campaign queue index.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php)[[4343](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php#L4343-L4372)]<br>#### `mailster_bounce`

###### **Records a hard or soft bounce for a subscriber and campaign.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber->ID` | `` | 
`$campaign_id` | `int` | Campaign ID.
`false` | `` | 
`$status` | `string|null` | Status value or filter.
`$index` | `int|null` | Campaign queue index.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php)[[4343](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php#L4343-L4391)]<br>

<hr>

#### `mailster_subscriber_change_status`

###### **Changes the status of one or more subscribers.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$new_status` | `int|string` | Target status ID or status name.
`$old_status` | `` | 
`$subscriber` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php)[[4632](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/subscribers.class.php#L4632-L4673)]<br>#### `mailster_trigger`

###### **Fires `mailster_trigger` for a single workflow, trigger, and subscriber.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$workflow_id` | `int` | Workflow post ID.
`$trigger` | `string` | Trigger slug.
`$subscriber` | `mixed` | Subscriber ID or object.

**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/automation.class.php)[[371](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/automation.class.php#L371-L383)]<br>

<hr>

#### `mailster_notice`

###### **Stores a new admin notice in the mailster_notices option.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$args['text']` | `` | 
`$args['type']` | `` | 
`$args['key']` | `` | 

**Changelog**

Version | Description
------- | -----------
`4.1.5` | 

Source: [./classes/notices.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/notices.class.php)[[130](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/notices.class.php#L130-L210)]<br>

<hr>

#### `mailster_remove_notice`

###### **Removes one or more stored notices by key.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$id` | `` | 

**Changelog**

Version | Description
------- | -----------
`4.1.5` | 

Source: [./classes/notices.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/notices.class.php)[[215](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/notices.class.php#L215-L236)]<br>#### `mailster_campaign_pause`

###### **Pauses an active or queued campaign, optionally at a future timestamp.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$id` | `int` | Campaign ID.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php)[[2946](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php#L2946-L2975)]<br>#### `mailster_campaign_start`

###### **Starts or schedules a campaign for delivery.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$id` | `int` | Campaign ID.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php)[[2983](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php#L2983-L3027)]<br>#### `mailster_campaign_start`

###### **Resumes a paused campaign, optionally at a future timestamp.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$id` | `int` | Campaign ID.

**Changelog**

Version | Description
------- | -----------
`2.4.10` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php)[[3037](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php#L3037-L3084)]<br>#### `mailster_finish_campaign`

###### **Marks a campaign finished and clears its queue, optionally scheduled.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$id` | `int` | Campaign ID.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php)[[3094](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php#L3094-L3174)]<br>

<hr>

#### `mailster_remove_notice_{$id}`

###### **Removes one or more stored notices by key.**


**Changelog**

Version | Description
------- | -----------
`4.1.5` | 

Source: [./classes/notices.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/notices.class.php)[[215](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/notices.class.php#L215-L237)]<br>

<hr>

#### `mailster_trigger_anniversary`

###### **Refreshes triggers, cleans orphan steps, and schedules after a workflow save.**


**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/automation.class.php)[[386](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/automation.class.php#L386-L418)]<br>

<hr>

#### `mailster_trigger_date`

###### **Refreshes triggers, cleans orphan steps, and schedules after a workflow save.**


**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/automation.class.php)[[386](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/automation.class.php#L386-L421)]<br>

<hr>

#### `mailster_list_save`

###### **Processes list create/update/delete form submissions on the detail screen.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$list_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/lists.class.php)[[199](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/lists.class.php#L199-L239)]<br>#### `mailster_update_list`

###### **Inserts or updates a list row and optionally assigns subscribers.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$list_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/lists.class.php)[[333](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/lists.class.php#L333-L416)]<br>

<hr>

#### `mailster_list_delete`

###### **Processes list create/update/delete form submissions on the detail screen.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$list->ID` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/lists.class.php)[[199](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/lists.class.php#L199-L250)]<br>

<hr>

#### `mailster_list_confirmed`

###### **Sets the list membership `added` timestamp to confirm a subscriber.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$list_id` | `int` | List id.
`$subscriber_id` | `int` | Subscriber id.
`$added` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/lists.class.php)[[544](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/lists.class.php#L544-L576)]<br>#### `mailster_list_added`

###### **Inserts a list–subscriber relationship and fires assignment hooks.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$list_id` | `int` | List id.
`$subscriber_id` | `int` | Subscriber id.
`$added` | `int|bool|null` | Confirmation timestamp or flag. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/lists.class.php)[[696](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/lists.class.php#L696-L740)]<br>#### `mailster_list_confirmed`

###### **Inserts a list–subscriber relationship and fires assignment hooks.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$list_id` | `int` | List id.
`$subscriber_id` | `int` | Subscriber id.
`$added` | `int|bool|null` | Confirmation timestamp or flag. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/lists.class.php)[[696](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/lists.class.php#L696-L743)]<br>

<hr>

#### `mailster_send`

###### **Sends a campaign email to a subscriber with tracking and tags.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber->ID` | `` | 
`$campaign->ID` | `` | 
`$campaignindex` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php)[[5443](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php#L5443-L5627)]<br>

<hr>

#### `mailster_subscriber_error`

###### **Sends a campaign email to a subscriber with tracking and tags.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber->ID` | `` | 
`$campaign->ID` | `` | 
`$mail->last_error->getMessage()` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php)[[5443](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php#L5443-L5639)]<br>#### `mailster_system_error`

###### **Sends a campaign email to a subscriber with tracking and tags.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber->ID` | `` | 
`$campaign->ID` | `` | 
`$mail->last_error->getMessage()` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php)[[5443](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php#L5443-L5647)]<br>#### `mailster_campaign_error`

###### **Sends a campaign email to a subscriber with tracking and tags.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber->ID` | `` | 
`$campaign->ID` | `` | 
`$mail->last_error->getMessage()` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php)[[5443](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php#L5443-L5655)]<br>

<hr>

#### `mailster_iframe_script_styles`

###### **Returns script and style tags for the campaign editor iframe.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php)[[6256](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php#L6256-L6405)]<br>

<hr>

#### `mailster_iframe_body`

###### **Returns extra body markup for the campaign editor iframe.**


**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php)[[6415](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/campaigns.class.php#L6415-L6430)]<br>

<hr>

#### `mailster_add_style`

###### **Returns or echoes the front-end Mailster form stylesheet markup.**


**Changelog**

Version | Description
------- | -----------
`2.3.17` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/helper.class.php)[[1392](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/helper.class.php#L1392-L1406)]<br>

<hr>

#### `mailster_form_head_button`

###### **Prints styles for iframe, embed, button, or editable form heads.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php)[[103](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php#L103-L128)]<br>

<hr>

#### `mailster_form_head_embeded`

###### **Prints styles for iframe, embed, button, or editable form heads.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php)[[103](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php#L103-L138)]<br>

<hr>

#### `mailster_form_head_iframe`

###### **Prints styles for iframe, embed, button, or editable form heads.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php)[[103](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php#L103-L144)]<br>

<hr>

#### `mailster_form_body_button`

###### **Renders the form body for button, iframe, editable, or embed contexts.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php)[[153](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php#L153-L166)]<br>

<hr>

#### `mailster_form_body_iframe`

###### **Renders the form body for button, iframe, editable, or embed contexts.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php)[[153](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php#L153-L171)]<br>

<hr>

#### `mailster_form_footer_button`

###### **Prints scripts for iframe, embed, button, or editable form footers.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php)[[196](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php#L196-L213)]<br>

<hr>

#### `mailster_form_footer_embeded`

###### **Prints scripts for iframe, embed, button, or editable form footers.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php)[[196](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php#L196-L223)]<br>

<hr>

#### `mailster_form_footer_iframe`

###### **Prints scripts for iframe, embed, button, or editable form footers.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php)[[196](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php#L196-L228)]<br>

<hr>

#### `mailster_form_delete`

###### **Saves form detail POST data (structure, design, settings, or delete).**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$form->ID` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php)[[468](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php#L468-L588)]<br>

<hr>

#### `mailster_update_form`

###### **Updates a form row and optionally reassigns lists.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$form_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php)[[724](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php#L724-L765)]<br>#### `mailster_add_form`

###### **Inserts a new form with defaults and returns its ID.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$form_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php)[[778](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php#L778-L840)]<br>

<hr>

#### `mailster_unassign_form_lists`

###### **Removes list assignments from forms, optionally scoped by list IDs.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$form_ids` | `int|int[]` | Form ID or IDs.
`$lists` | `int|int[]|null` | Lists to remove; null means all. (optional).
`$not_list` | `int|int[]|null` | Lists to keep when clearing others. (optional).

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php)[[1067](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php#L1067-L1102)]<br>

<hr>

#### `mailster_unassign_form_tags`

###### **Removes tag assignments from forms, optionally scoped by tag IDs.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$form_ids` | `int|int[]` | Form ID or IDs.
`$tags` | `int|int[]|null` | Tags to remove; null means all. (optional).
`$not_tag` | `int|int[]|null` | Tags to keep when clearing others. (optional).

**Changelog**

Version | Description
------- | -----------
`3.0` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php)[[1167](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/forms.class.php#L1167-L1202)]<br>

<hr>

#### `mailster_form_{$type}`

###### **Persists a form analytics action row.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$form_id` | `int` | Form post ID.
`$subscriber_id` | `int|null` | Subscriber ID.
`$entry->post_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/block-forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/block-forms.class.php)[[2445](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/block-forms.class.php#L2445-L2488)]<br>

<hr>

#### `mailster_form_{$type}`

###### **Persists a form analytics action row.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$form_id` | `int` | Form post ID.
`$subscriber_id` | `int|null` | Subscriber ID.
`$post_id` | `int|null` | Related post ID.

**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/block-forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/block-forms.class.php)[[2445](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/block-forms.class.php#L2445-L2504)]<br>

<hr>

#### `mailster_{$action}`

###### **Installs, activates, or configures a Mailster add-on during quick install steps.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$args` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/ajax.class.php](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/ajax.class.php)[[3354](https://github.com/everpress-co/mailster/blob/4.1.20/./classes/ajax.class.php#L3354-L3389)]<br>



