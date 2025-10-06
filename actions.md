# Actions
Mailster provides various hooks and filters you can use to alter the behavior of the plugin or write your own add-ons and extensions. We recommend to read more about hooks on the [official site](https://developer.wordpress.org/plugins/hooks/).

!>  While there are more hooks in the plugin we only list a few here.

<hr>

#### `mailster_remove_notice`

###### **Remove a notice**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$id` | `` | 

Source: [./classes/notices.class.php](https://github.com/everpress-co/mailster/blob/4.1.13/./classes/notices.class.php)[[162](https://github.com/everpress-co/mailster/blob/4.1.13/./classes/notices.class.php#L162-L181)]<br>

<hr>

#### `mailster_remove_notice_{$id}`

###### **Remove a notice**


Source: [./classes/notices.class.php](https://github.com/everpress-co/mailster/blob/4.1.13/./classes/notices.class.php)[[162](https://github.com/everpress-co/mailster/blob/4.1.13/./classes/notices.class.php#L162-L182)]<br>

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

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.13/./classes/frontpage.class.php)[[429](https://github.com/everpress-co/mailster/blob/4.1.13/./classes/frontpage.class.php#L429-L438)]<br>#### `mailster_open`

###### **Fires if user opens on a campaign and tracking is enabled**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `int` | The ID of the subscriber
`$campaign_id` | `int` | Form The ID of the campaign
`$campaign_index` | `int` | The index of the campaign

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.13/./classes/frontpage.class.php)[[442](https://github.com/everpress-co/mailster/blob/4.1.13/./classes/frontpage.class.php#L442-L449)]<br>

<hr>

#### `mailster_subscriber_subscribed`

###### **Run after the users confirms the subscription**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `int` | The ID of the subscriber

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.13/./classes/frontpage.class.php)[[649](https://github.com/everpress-co/mailster/blob/4.1.13/./classes/frontpage.class.php#L649-L654)]<br>

<hr>

#### `mailster_check_bounces`

###### **Checks for new newsletter in the queue to start new cronjob**


Source: [./classes/cron.class.php](https://github.com/everpress-co/mailster/blob/4.1.13/./classes/cron.class.php)[[31](https://github.com/everpress-co/mailster/blob/4.1.13/./classes/cron.class.php#L31-L37)]<br>

<hr>

#### `mailster_resend_confirmations`

###### **Checks for new newsletter in the queue to start new cronjob**


Source: [./classes/cron.class.php](https://github.com/everpress-co/mailster/blob/4.1.13/./classes/cron.class.php)[[31](https://github.com/everpress-co/mailster/blob/4.1.13/./classes/cron.class.php#L31-L40)]<br>



