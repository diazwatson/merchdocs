---
title: Now Online
---

The Now Online option on the Customers menu lists all customers and visitors who are currently online in your store. The interval of time that customers are shown as currently online is set in the configuration, and determines how long the customer’s activity is visible from the Admin. By default, the interval is fifteen minutes.

![]({{ site.baseurl }}{% link images/images/customers-now-online.png %}){: .zoom}
[_Online Customers_]({{ site.baseurl }}{% link configuration/customers/customer-configuration.md %})

## To see all customers who are online now:

1. On the _Admin_ sidebar, go to **Customers** > **Online Now**.

1. To help an online customer complete a purchase, see [Shopping Assistance]({{ site.baseurl }}{% link sales/shopping-assistance.md %}).

## To configure the time interval:

1. On the _Admin_ sidebar, go to **Stores** > _Settings_ > **Configuration**.

1. In the panel on the left, expand **Customers** and choose **Customer Configuration**.

1. Expand ![]({{ site.baseurl }}{% link images/images/btn-expand.png %}){: .Inline} the **Online Customers Options** section. Then, do the following:

      ![]({{ site.baseurl }}{% link images/images/config-customers-customer-configuration-online-customers-options.png %}){: .zoom}
      [_Online Customers Options_]({{ site.baseurl }}{% link configuration/customers/customer-configuration.md %})

      - In the **Online Minutes Interval** field, enter the number of minutes for the customer session to be visible from the Admin. Leave the field empty to accept the default interval of fifteen minutes.
  
      - In the **Customer Data Lifetime** field, enter the number of minutes before any unsaved data entered by the customer expires.

1. When complete, click <span class="btn">Save Config</span>.

## Column Descriptions

| Column             | Description                                                                              |
|--------------------|------------------------------------------------------------------------------------------|
| ID                 | The customer ID of a registered customer.                                                |
| First Name         | The first name of a registered customer.                                                 |
| Last Name          | The last name of a registered customer.                                                  |
| Email              | The email address of a registered customer.                                              |
| IP Address         | The IP address of the computer that customers and guests are using to access your store. |
| Session Start Time | The date and time that marks the beginning of the current customer session.              |
| Last Activity      | The date and time of the customer’s last activity in your store.                         |
| Type               | Options: Customer / Visitor                                                      |
| Last URL           | The last URL the customer visited.                                                       |
