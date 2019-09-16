---
title: Resolving Account Errors
---


Your account may be disapproved or suspended due to breaking the Google [Terms of Service][1] and policies on [Prohibited Content][2]. The following instructions and information help you review and resolve your account issues. Some of the issues that can cause disapprovals may include product issues. When you open an error, the issue displays with additional information and a link to Google policies and instructions. Review the information then complete edits and actions to resolve those issues through the Magento Admin.

Review Google's [Understanding account suspension][3], [best practices]({{ site.baseurl }}{% link sales-channels/google-ads/google-best-practices.md %}), and [troubleshooting][4] for additional information.

After onboarding completes, we check for product approval and account status with Google every 30 minutes for the first 72 hours of your integration. Google may require up to 10 days to complete reviews. After the first 72 hours, Magento checks product and account status once every 24 hours.

{:.bs-callout .bs-callout-tip}
You can also check the service log for additional information when troubleshooting is needed. Google Shopping ads Channel logging is written to the `{Magento Root}/var/log/google_indexer.log` file and can be viewed in [developer mode]({{ site.baseurl }}{% link magento/installation-modes.md %}). Information for this log includes requests to and responses from Google. To enable or disable logging, see [Channels]({{ site.baseurl }}{% link configuration/services/channels.md %}).

## To resolve account errors:

1. On the Admin sidebar, click **Marketing**. Then under Advertising Channels, click **Google Shopping ads**.

1. In the GMC Accounts table, locate an account with Account Status of "Disapproved". In the **Actions** column, click **Views Details**.

1. Click **Account Disapprovals**. A list of all account issues displays.

    ![]({{ site.baseurl }}{% link images/images/sales-channels/google/account-disapproved-list.png %}){: .zoom}
    *Account Disapprovals*

1. For each issue, click **Read Google guidelines**in the **Actions** column. Complete any changes required to resolve the issue.

[1]: https://support.google.com/merchants/answer/160173?hl=en
[2]: https://support.google.com/merchants/answer/6149970?hl=en
[3]: https://support.google.com/merchants/answer/2948694
[4]: https://support.magento.com/hc/en-us/articles/360026926371
