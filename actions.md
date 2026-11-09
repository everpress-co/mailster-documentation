# Actions
Mailster provides various hooks and filters you can use to alter the behavior of the plugin or write your own add-ons and extensions. We recommend to read more about hooks on the [official site](https://developer.wordpress.org/plugins/hooks/).

!>  While there are more hooks in the plugin we only list a few here.

<hr>

#### `mailster_subscriber_save`

###### **Handles create and update submissions on the subscriber edit screen.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[481](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L481-L510)]<br>#### `mailster_update_subscriber`

###### **Updates an existing subscriber or creates one when missing.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[1136](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L1136-L1325)]<br>#### `mailster_add_subscriber`

###### **Adds a new subscriber, optionally overwriting or merging an existing one.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[1353](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L1353-L1420)]<br>#### `mailster_subscriber_subscribed`

###### **Run after the users confirms the subscription**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `int` | The ID of the subscriber

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php)[[730](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php#L730-L735)]<br>#### `mailster_list_unconfirmed`

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

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php)[[624](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php#L624-L651)]<br>#### `mailster_list_removed`

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

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php)[[790](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php#L790-L817)]<br>

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

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[481](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L481-L611)]<br>

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

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[481](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L481-L633)]<br>#### `mailster_subscriber_delete`

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

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[481](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L481-L668)]<br>

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

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[1592](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L1592-L1650)]<br>

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

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[1661](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L1661-L1712)]<br>#### `mailster_remove_custom_field`

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

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[1723](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L1723-L1751)]<br>

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

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[3288](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L3288-L3331)]<br>#### `mailster_unsubscribe`

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

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[3288](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L3288-L3351)]<br>#### `mailster_bounce`

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

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[4384](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L4384-L4413)]<br>#### `mailster_bounce`

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

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[4384](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L4384-L4432)]<br>

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

Source: [./classes/subscribers.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php)[[4673](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/subscribers.class.php#L4673-L4714)]<br>#### `mailster_trigger`

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

Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php)[[374](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php#L374-L386)]<br>

<hr>

#### `mailster_campaign_pause`

###### **Pauses an active or queued campaign, optionally at a future timestamp.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$id` | `int` | Campaign ID.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[2954](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L2954-L2983)]<br>#### `mailster_campaign_start`

###### **Starts or schedules a campaign for delivery.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$id` | `int` | Campaign ID.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[2991](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L2991-L3035)]<br>#### `mailster_campaign_start`

###### **Resumes a paused campaign, optionally at a future timestamp.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$id` | `int` | Campaign ID.

**Changelog**

Version | Description
------- | -----------
`2.4.10` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[3045](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L3045-L3092)]<br>#### `mailster_finish_campaign`

###### **Marks a campaign finished and clears its queue, optionally scheduled.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$id` | `int` | Campaign ID.

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[3102](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L3102-L3182)]<br>#### `mailster_remove_notice`

###### **Removes one or more stored notices by key.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$id` | `` | 

**Changelog**

Version | Description
------- | -----------
`4.1.5` | 

Source: [./classes/notices.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notices.class.php)[[216](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notices.class.php#L216-L237)]<br>

<hr>

#### `mailster_campaign_duplicate`

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

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[3192](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L3192-L3262)]<br>#### `mailster_autoresponder_post_published`

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

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[5920](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L5920-L6025)]<br>#### `mailster_workflow_duplicate`

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

Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php)[[1939](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php#L1939-L1997)]<br>#### `mailster_form_duplicate`

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

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[851](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L851-L899)]<br>#### `mailster_autoresponder_post_published`

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

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php)[[416](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php#L416-L692)]<br>#### `mailster_autoresponder_timebased`

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

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php)[[712](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php#L712-L852)]<br>

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

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[5498](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L5498-L5682)]<br>

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

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[5498](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L5498-L5694)]<br>#### `mailster_system_error`

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

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[5498](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L5498-L5702)]<br>#### `mailster_campaign_error`

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

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[5498](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L5498-L5710)]<br>

<hr>

#### `mailster_iframe_script_styles`

###### **Returns script and style tags for the campaign editor iframe.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[6311](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L6311-L6460)]<br>

<hr>

#### `mailster_iframe_body`

###### **Returns extra body markup for the campaign editor iframe.**


**Changelog**

Version | Description
------- | -----------
`2.3` | 

Source: [./classes/campaigns.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php)[[6470](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/campaigns.class.php#L6470-L6485)]<br>

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

Source: [./classes/notices.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notices.class.php)[[131](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notices.class.php#L131-L211)]<br>

<hr>

#### `mailster_remove_notice_{$id}`

###### **Removes one or more stored notices by key.**


**Changelog**

Version | Description
------- | -----------
`4.1.5` | 

Source: [./classes/notices.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notices.class.php)[[216](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notices.class.php#L216-L238)]<br>

<hr>

#### `mailster_add_tag`

###### **Replaces static placeholders, custom tags, and fallbacks.**


**Changelog**

Version | Description
------- | -----------
`2.3.12` | 

Source: [./classes/placeholder.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php)[[1336](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/placeholder.class.php#L1336-L1349)]<br>Source: [./classes/tinymce.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tinymce.class.php)[[72](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tinymce.class.php#L72-L87)]<br>

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

Source: [./classes/tags.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tags.class.php)[[41](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tags.class.php#L41-L106)]<br>

<hr>

#### `mailster_tag_added`

###### **Assigns a single tag to a single subscriber.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$tag_id` | `` | 
`$subscriber_id` | `int` | Subscriber ID.
`$name` | `` | 

**Changelog**

Version | Description
------- | -----------
`3.0` | 

Source: [./classes/tags.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tags.class.php)[[294](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tags.class.php#L294-L326)]<br>#### `mailster_tag_removed`

###### **Unassigns a single tag from a single subscriber.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$tag_id` | `` | 
`$subscriber_id` | `int` | Subscriber ID.
`$name` | `` | 

**Changelog**

Version | Description
------- | -----------
`3.0` | 

Source: [./classes/tags.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tags.class.php)[[374](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/tags.class.php#L374-L408)]<br>

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

Source: [./classes/ajax.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php)[[3404](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php#L3404-L3439)]<br>

<hr>

#### `mailster_cron`

###### **Saves a setup wizard step options payload and returns success JSON.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/ajax.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php)[[3459](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/ajax.class.php#L3459-L3522)]<br>Source: [./classes/dashboard.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/dashboard.class.php)[[75](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/dashboard.class.php#L75-L89)]<br>

<hr>

#### `mailster_trigger_anniversary`

###### **Refreshes triggers, cleans orphan steps, and schedules after a workflow save.**


**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php)[[389](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php#L389-L423)]<br>

<hr>

#### `mailster_trigger_date`

###### **Refreshes triggers, cleans orphan steps, and schedules after a workflow save.**


**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php)[[389](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php#L389-L426)]<br>

<hr>

#### `mailster_admin_header`

###### **Enqueues CSS for the workflows admin list screen.**


**Changelog**

Version | Description
------- | -----------
`4.0.0` | 

Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php)[[1578](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php#L1578-L1598)]<br>Source: [./classes/automation.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php)[[1603](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/automation.class.php#L1603-L1618)]<br>Source: [./classes/health.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/health.class.php)[[47](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/health.class.php#L47-L56)]<br>Source: [./classes/block-forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/block-forms.class.php)[[1441](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/block-forms.class.php#L1441-L1461)]<br>Source: [./classes/block-forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/block-forms.class.php)[[1470](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/block-forms.class.php#L1470-L1485)]<br>Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[1283](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L1283-L1301)]<br>Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[1545](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L1545-L1559)]<br>Source: [./classes/upgrade.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/upgrade.class.php)[[496](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/upgrade.class.php#L496-L507)]<br>

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

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php)[[103](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php#L103-L116)]<br>

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

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php)[[471](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php#L471-L480)]<br>#### `mailster_open`

###### **Fires if user opens on a campaign and tracking is enabled**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `int` | The ID of the subscriber
`$campaign_id` | `int` | Form The ID of the campaign
`$campaign_index` | `int` | The index of the campaign

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php)[[484](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php#L484-L491)]<br>

<hr>

#### `mailster_homepage_subscribe`

###### **Handles subscribe, unsubscribe, profile, and confirm homepage subpages.**


**Changelog**

Version | Description
------- | -----------
`2.2.8` | 

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php)[[559](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php#L559-L578)]<br>

<hr>

#### `mailster_homepage_unsubscribe`

###### **Handles subscribe, unsubscribe, profile, and confirm homepage subpages.**


**Changelog**

Version | Description
------- | -----------
`2.2.8` | 

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php)[[559](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php#L559-L614)]<br>

<hr>

#### `mailster_homepage_profile`

###### **Handles subscribe, unsubscribe, profile, and confirm homepage subpages.**


**Changelog**

Version | Description
------- | -----------
`2.2.8` | 

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php)[[559](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php#L559-L630)]<br>

<hr>

#### `mailster_homepage_confirm`

###### **Handles subscribe, unsubscribe, profile, and confirm homepage subpages.**


**Changelog**

Version | Description
------- | -----------
`2.2.8` | 

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php)[[559](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php#L559-L653)]<br>

<hr>

#### `mailster_frontpage`

###### **Renders a single newsletter web version with or without the frame chrome.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php)[[818](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php#L818-L840)]<br>

<hr>

#### `mailster_frontpage_frame`

###### **Renders a single newsletter web version with or without the frame chrome.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php)[[818](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/frontpage.class.php#L818-L891)]<br>

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

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php)[[200](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php#L200-L240)]<br>#### `mailster_update_list`

###### **Inserts or updates a list row and optionally assigns subscribers.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$list_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php)[[334](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php#L334-L417)]<br>

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

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php)[[200](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php#L200-L251)]<br>

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

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php)[[545](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php#L545-L577)]<br>#### `mailster_list_added`

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

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php)[[697](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php#L697-L741)]<br>#### `mailster_list_confirmed`

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

Source: [./classes/lists.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php)[[697](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/lists.class.php#L697-L744)]<br>

<hr>

#### `mailster_add_style`

###### **Returns or echoes the front-end Mailster form stylesheet markup.**


**Changelog**

Version | Description
------- | -----------
`2.3.17` | 

Source: [./classes/helper.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php)[[1393](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/helper.class.php#L1393-L1407)]<br>

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

Source: [./classes/notification.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php)[[528](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/notification.class.php#L528-L569)]<br>

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

Source: [./classes/block-forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/block-forms.class.php)[[2453](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/block-forms.class.php#L2453-L2496)]<br>

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

Source: [./classes/block-forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/block-forms.class.php)[[2453](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/block-forms.class.php#L2453-L2512)]<br>

<hr>

#### `mailster_freemius_loaded`

###### **Initializes and returns the Freemius SDK instance.**


**Changelog**

Version | Description
------- | -----------
`3.3.0` | 

Source: [./classes/license.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/license.class.php)[[50](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/license.class.php#L50-L93)]<br>

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

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[324](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L324-L372)]<br>#### `mailster_initsend`

###### **Configures the mailer transport, DKIM, limits, and error classifiers.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mail.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.class.php)[[413](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.class.php#L413-L468)]<br>#### `mailster_presend`

###### **Runs presend/dosend hooks and returns the Message-ID when sent.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mail.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.class.php)[[992](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.class.php#L992-L1010)]<br>#### `mailster_dosend`

###### **Runs presend/dosend hooks and returns the Message-ID when sent.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$this` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mail.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.class.php)[[992](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mail.class.php#L992-L1016)]<br>

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

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[1343](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L1343-L1403)]<br>

<hr>

#### `mailster_thirdpartystuff`

###### **Hooks third-party cache flush helpers on shutdown.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/mailster.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php)[[3607](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/mailster.class.php#L3607-L3616)]<br>

<hr>

#### `mailster_form_head_button`

###### **Prints styles for iframe, embed, button, or editable form heads.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[104](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L104-L129)]<br>

<hr>

#### `mailster_form_head_embeded`

###### **Prints styles for iframe, embed, button, or editable form heads.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[104](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L104-L139)]<br>

<hr>

#### `mailster_form_head_iframe`

###### **Prints styles for iframe, embed, button, or editable form heads.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[104](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L104-L145)]<br>

<hr>

#### `mailster_form_body_button`

###### **Renders the form body for button, iframe, editable, or embed contexts.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[154](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L154-L167)]<br>

<hr>

#### `mailster_form_body_iframe`

###### **Renders the form body for button, iframe, editable, or embed contexts.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[154](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L154-L172)]<br>

<hr>

#### `mailster_form_footer_button`

###### **Prints scripts for iframe, embed, button, or editable form footers.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[197](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L197-L214)]<br>

<hr>

#### `mailster_form_footer_embeded`

###### **Prints scripts for iframe, embed, button, or editable form footers.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[197](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L197-L224)]<br>

<hr>

#### `mailster_form_footer_iframe`

###### **Prints scripts for iframe, embed, button, or editable form footers.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[197](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L197-L229)]<br>

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

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[469](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L469-L586)]<br>

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

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[724](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L724-L765)]<br>#### `mailster_add_form`

###### **Inserts a new form with defaults and returns its ID.**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$form_id` | `` | 

**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[778](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L778-L840)]<br>

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

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[1067](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L1067-L1102)]<br>

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

Source: [./classes/forms.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php)[[1167](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/forms.class.php#L1167-L1202)]<br>

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

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php)[[873](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php#L873-L1022)]<br>

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

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php)[[1062](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php#L1062-L1366)]<br>#### `mailster_notification_error`

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

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php)[[1062](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php#L1062-L1383)]<br>#### `mailster_campaign_error`

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

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php)[[1062](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php#L1062-L1404)]<br>#### `mailster_system_error`

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

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php)[[1062](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php#L1062-L1410)]<br>

<hr>

#### `mailster_cron_finished`

###### **Processes due queue entries: sends campaign and notification emails for this cron turn.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/queue.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php)[[1062](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/queue.class.php#L1062-L1499)]<br>

<hr>

#### `mailster_precheck_script_styles`

###### **Prints and returns the Precheck editor CSS and JavaScript assets.**


**Changelog**

Version | Description
------- | -----------
`3.0` | 

Source: [./classes/precheck.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/precheck.class.php)[[18](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/precheck.class.php#L18-L38)]<br>

<hr>

#### `mailster_check_bounces`

###### **Hourly maintenance: bounce check, resend confirmations, and refresh schedules.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/cron.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/cron.class.php)[[48](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/cron.class.php#L48-L58)]<br>

<hr>

#### `mailster_resend_confirmations`

###### **Hourly maintenance: bounce check, resend confirmations, and refresh schedules.**


**Changelog**

Version | Description
------- | -----------
`2.2` | 

Source: [./classes/cron.class.php](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/cron.class.php)[[48](https://github.com/everpress-co/mailster/blob/4.1.22/./classes/cron.class.php#L48-L61)]<br>



