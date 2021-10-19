# Cron Job

All of your campaigns are sent via a cronjob. There are two cron services available:

## wp_cron

This is the cron service which is built right into WordPress. If you choose this option you don't have to set up anything else to get your campaign sent. You only have to visit your blog (backend or frontend) regularly to trigger the cron.

Read more about the WordPress cron service [here](http://wp.tutsplus.com/articles/insights-into-wp-cron-an-introduction-to-scheduling-tasks-in-wordpress/).

!> This type of service is not recommended for many subscribers!

## Real cron service

Much better is a real cron service offered by your hosting provider.

You have to call a specific URL which looks like:

?> `https://example.com/mailster/12b690fc32e85fe810b772e657cc3719`

You can find your URL in the Newsletter Settings page within the "[Cron](/settings/cron)" tab.

You can trigger the cron in three ways:

1. Open the mentioned link in a browser - which refreshes every x minutes and triggers the job for you.
2. Let a third part site trigger (which opens the page like your did) which are sometimes free.
3. Tell your provider or host to trigger them for you (same thing but technically slightly different).

### There are also some free service out there:

-   https://www.easycron.com/
-   https://cron-job.org/en/
-   https://www.setcronjob.com/
-   http://www.onlinecronjobs.com/
