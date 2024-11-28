# Actions
Mailster provides various hooks and filters you can use to alter the behavior of the plugin or write your own add-ons and extensions. We recommend to read more about hooks on the [official site](https://developer.wordpress.org/plugins/hooks/).

!>  While there are more hooks in the plugin we only list a few here.

<hr>

#### `mailster_send`

###### **These tests prove test setup works.**

They are useful for debugging.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`1` |  | 
`1` |  | 

Source: [./tests/Integration/ActionsTest.php](https://github.com/everpress-co/mailster/blob/4.1.6/./tests/Integration/ActionsTest.php)[[9](https://github.com/everpress-co/mailster/blob/4.1.6/./tests/Integration/ActionsTest.php#L9-L22)]<br>

<hr>

#### `mailster_open`

###### **These tests prove test setup works.**

They are useful for debugging.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`1` |  | 
`1` |  | 

Source: [./tests/Integration/ActionsTest.php](https://github.com/everpress-co/mailster/blob/4.1.6/./tests/Integration/ActionsTest.php)[[9](https://github.com/everpress-co/mailster/blob/4.1.6/./tests/Integration/ActionsTest.php#L9-L31)]<br>Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.6/./classes/frontpage.class.php)[[442](https://github.com/everpress-co/mailster/blob/4.1.6/./classes/frontpage.class.php#L442-L449)]<br>

<hr>

#### `mailster_click`

###### **These tests prove test setup works.**

They are useful for debugging.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`1` |  | 
`1` |  | 
`'http://google.com'` |  | 

Source: [./tests/Integration/ActionsTest.php](https://github.com/everpress-co/mailster/blob/4.1.6/./tests/Integration/ActionsTest.php)[[9](https://github.com/everpress-co/mailster/blob/4.1.6/./tests/Integration/ActionsTest.php#L9-L40)]<br>Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.6/./classes/frontpage.class.php)[[429](https://github.com/everpress-co/mailster/blob/4.1.6/./classes/frontpage.class.php#L429-L438)]<br>

<hr>

#### `mailster_unsubscribe`

###### **These tests prove test setup works.**

They are useful for debugging.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`1` |  | 
`1` |  | 

Source: [./tests/Integration/ActionsTest.php](https://github.com/everpress-co/mailster/blob/4.1.6/./tests/Integration/ActionsTest.php)[[9](https://github.com/everpress-co/mailster/blob/4.1.6/./tests/Integration/ActionsTest.php#L9-L49)]<br>

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

Source: [./tests/Integration/ActionsTest.php](https://github.com/everpress-co/mailster/blob/4.1.6/./tests/Integration/ActionsTest.php)[[9](https://github.com/everpress-co/mailster/blob/4.1.6/./tests/Integration/ActionsTest.php#L9-L58)]<br>Source: [./tests/Integration/ActionsTest.php](https://github.com/everpress-co/mailster/blob/4.1.6/./tests/Integration/ActionsTest.php)[[9](https://github.com/everpress-co/mailster/blob/4.1.6/./tests/Integration/ActionsTest.php#L9-L66)]<br>

<hr>

#### `mailster_remove_notice`

###### **Remove a notice**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$id` |  | 

Source: [./classes/notices.class.php](https://github.com/everpress-co/mailster/blob/4.1.6/./classes/notices.class.php)[[162](https://github.com/everpress-co/mailster/blob/4.1.6/./classes/notices.class.php#L162-L181)]<br>

<hr>

#### `mailster_remove_notice_{$id}`

###### **Remove a notice**


Source: [./classes/notices.class.php](https://github.com/everpress-co/mailster/blob/4.1.6/./classes/notices.class.php)[[162](https://github.com/everpress-co/mailster/blob/4.1.6/./classes/notices.class.php#L162-L182)]<br>

<hr>

#### `mailster_subscriber_subscribed`

###### **Run after the users confirms the subscription**

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`$subscriber_id` | `int` | The ID of the subscriber

Source: [./classes/frontpage.class.php](https://github.com/everpress-co/mailster/blob/4.1.6/./classes/frontpage.class.php)[[649](https://github.com/everpress-co/mailster/blob/4.1.6/./classes/frontpage.class.php#L649-L654)]<br>

<hr>

#### `mailster_check_bounces`

###### **Checks for new newsletter in the queue to start new cronjob**


Source: [./classes/cron.class.php](https://github.com/everpress-co/mailster/blob/4.1.6/./classes/cron.class.php)[[31](https://github.com/everpress-co/mailster/blob/4.1.6/./classes/cron.class.php#L31-L37)]<br>

<hr>

#### `mailster_resend_confirmations`

###### **Checks for new newsletter in the queue to start new cronjob**


Source: [./classes/cron.class.php](https://github.com/everpress-co/mailster/blob/4.1.6/./classes/cron.class.php)[[31](https://github.com/everpress-co/mailster/blob/4.1.6/./classes/cron.class.php#L31-L40)]<br>



