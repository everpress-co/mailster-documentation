# Shortcodes

Mailster supports **five** built in shortcodes you can use. You can use them anywhere where shortcodes are accepted.

### `[newsletter]`

Embeds a newsletter campaign as iframe.

Attribute|Default|Option
--|--|--
id|`null`|The ID of the campaign
scrolling|`true`| sets the scrolling of the iframe

##### Example
```
[newsletter id=1]
```

### `[newsletter_list]`

Displays a list of links to your latest newsletters.

Attribute|Default|Option
--|--|--
date|`false`|Display date next to the link
count|`10`|Number of list items
status|`(array)( 'finished', 'active' )`|Status of campaigns
order|`'desc'`|Order direction ('asc' or 'desc')
orderby|`'date'`|Order by value


##### Example
```
[newsletter_list count=3 order="post_name"]
```

### `[newsletter_signup_form]`

Displays a newsletter sign up form with a certain id.

Attribute|Default|Option
--|--|--
id|`null`|The ID of the form.


##### Example
```
[newsletter_signup_form id=3]
```

### `[newsletter_subscribers]`

Displays the number of your subscribers.

Attribute|Default|Option
--|--|--
formatted|`true`|formats the number with [`number_format_i18n()`](https://codex.wordpress.org/Function_Reference/number_format_i18n)
round|`1`|Round up to the next X value (eg. 10, 100, 1000, etc.)
lists|`null`|Display count from a certain list


##### Example
```
[newsletter_subscribers round=1000 lists"3,4,7"]
```

!> Counting the numbers of subscribers can be time consuming if you have many. Consider page caching to prevent slow responses on your site.

### `[newsletter_button]`

Displays a Subscriber Button.

Attribute|Default|Option
--|--|--
id|`null`|The ID of the form.
showcount| `false`|Display the number of your subscribers.
label|Content from Texts|The label of the button,
design| `'default'`|Currently supported style: 'default', 'wp', 'twitter', 'flat', 'minimal'
width| `480`|Width of the popup

##### Example
```
[newsletter_button id=3 showcount="true" label="Subscribe now!" design="wp"]
```
