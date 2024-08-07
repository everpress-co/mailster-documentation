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

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/blob/4.1.2/./classes/frontpage.class.php)[[429](https://github.com/evrpress/mailster/blob/4.1.2/./classes/frontpage.class.php#L429-L438)]<br>Source: [./tests/integration/ActionsTest.php](https://github.com/evrpress/mailster/blob/4.1.2/./tests/integration/ActionsTest.php)[[9](https://github.com/evrpress/mailster/blob/4.1.2/./tests/integration/ActionsTest.php#L9-L40)]<br>

<hr>

#### `mailster_open`

###### **Fires if user opens on a campaign and tracking is enabled**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `int` | The ID of the subscriber
`$campaign_id` | `int` | Form The ID of the campaign
`$campaign_index` | `int` | The index of the campaign

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/blob/4.1.2/./classes/frontpage.class.php)[[442](https://github.com/evrpress/mailster/blob/4.1.2/./classes/frontpage.class.php#L442-L449)]<br>Source: [./tests/integration/ActionsTest.php](https://github.com/evrpress/mailster/blob/4.1.2/./tests/integration/ActionsTest.php)[[9](https://github.com/evrpress/mailster/blob/4.1.2/./tests/integration/ActionsTest.php#L9-L31)]<br>

<hr>

#### `mailster_subscriber_subscribed`

###### **Run after the users confirms the subscription**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `int` | The ID of the subscriber

Source: [./classes/frontpage.class.php](https://github.com/evrpress/mailster/blob/4.1.2/./classes/frontpage.class.php)[[648](https://github.com/evrpress/mailster/blob/4.1.2/./classes/frontpage.class.php#L648-L653)]<br>

<hr>

#### `mailster_check_bounces`

###### **Checks for new newsletter in the queue to start new cronjob**


Source: [./classes/cron.class.php](https://github.com/evrpress/mailster/blob/4.1.2/./classes/cron.class.php)[[31](https://github.com/evrpress/mailster/blob/4.1.2/./classes/cron.class.php#L31-L37)]<br>

<hr>

#### `mailster_resend_confirmations`

###### **Checks for new newsletter in the queue to start new cronjob**


Source: [./classes/cron.class.php](https://github.com/evrpress/mailster/blob/4.1.2/./classes/cron.class.php)[[31](https://github.com/evrpress/mailster/blob/4.1.2/./classes/cron.class.php#L31-L40)]<br>

<hr>

#### `mailster_send`

###### **These tests prove test setup works.**

They are useful for debugging.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`1` |  | 
`1` |  | 

Source: [./tests/integration/ActionsTest.php](https://github.com/evrpress/mailster/blob/4.1.2/./tests/integration/ActionsTest.php)[[9](https://github.com/evrpress/mailster/blob/4.1.2/./tests/integration/ActionsTest.php#L9-L22)]<br>

<hr>

#### `mailster_unsubscribe`

###### **These tests prove test setup works.**

They are useful for debugging.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`1` |  | 
`1` |  | 

Source: [./tests/integration/ActionsTest.php](https://github.com/evrpress/mailster/blob/4.1.2/./tests/integration/ActionsTest.php)[[9](https://github.com/evrpress/mailster/blob/4.1.2/./tests/integration/ActionsTest.php#L9-L49)]<br>

<hr>

#### `mailster_bounce`

###### **These tests prove test setup works.**

They are useful for debugging.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`1` |  | 
`1` |  | 
`false` |  | 

Source: [./tests/integration/ActionsTest.php](https://github.com/evrpress/mailster/blob/4.1.2/./tests/integration/ActionsTest.php)[[9](https://github.com/evrpress/mailster/blob/4.1.2/./tests/integration/ActionsTest.php#L9-L58)]<br>Source: [./tests/integration/ActionsTest.php](https://github.com/evrpress/mailster/blob/4.1.2/./tests/integration/ActionsTest.php)[[9](https://github.com/evrpress/mailster/blob/4.1.2/./tests/integration/ActionsTest.php#L9-L66)]<br>



