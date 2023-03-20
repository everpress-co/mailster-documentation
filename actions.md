# Actions
Mailster provides various hooks and filters you can use to alter the behavior of the plugin or write your own add-ons and extensions. We recommend to read more about hooks on the [official site](https://developer.wordpress.org/plugins/hooks/).

!>  While there are more hooks in the plugin we only list a few here.

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

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/blob/3.3.1/./classes/frontpage.class.php)[[439](https://github.com/evrpress/mailster/blob/3.3.1/./classes/frontpage.class.php#L439-L448)]<br>

<hr>

#### `mailster_open`

###### **Fires if user opens on a campaign and tracking is enabled**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `int` | The ID of the subscriber
`$campaign_id` | `int` | Form The ID of the campaign
`$campaign_index` | `int` | The index of the campaign

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/blob/3.3.1/./classes/frontpage.class.php)[[454](https://github.com/evrpress/mailster/blob/3.3.1/./classes/frontpage.class.php#L454-L461)]<br>

<hr>

#### `mailster_subscriber_subscribed`

###### **Run after the users confirms the subscription**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `int` | The ID of the subscriber

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/blob/3.3.1/./classes/frontpage.class.php)[[640](https://github.com/evrpress/mailster/blob/3.3.1/./classes/frontpage.class.php#L640-L645)]<br>



