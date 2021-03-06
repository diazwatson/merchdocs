---
title: Persistent Shopping Cart
---

Stores > Settings > [Configuration]({{ site.baseurl }}{% link stores/configuration.md %}) > [Customers]({{ site.baseurl }}{% link configuration/customers.md %}) > Persistent Shopping Cart

## General Options

<!--{% if "Default.CE Only" contains site.edition %}-->
![]({{ site.baseurl }}{% link images/images/config-customers-persistent-shopping-cart-general-options.png %}){: .zoom}
[_General Options_]({{ site.baseurl }}{% link sales/cart-persistent-configuration.md %})
<!--{% endif %}-->
<!--{% if "Default.EE-B2B" contains site.edition %}-->
![]({{ site.baseurl }}{% link images/images-ee/config-customers-persistent-shopping-cart-general-options-ee.png %}){: .zoom}
[_General Options_]({{ site.baseurl }}{% link sales/cart-persistent-configuration.md %})
<!--{% endif %}-->

|Field|[Scope]({{ site.baseurl }}{% link configuration/scope.md %})|Description|
|--- |--- |--- |
|Enable Persistence|Website|Determines if  the persistence is enabled.|
|Persistence Lifetime (seconds)|Website|Defines the lifetime of the persistent cookie in seconds. Maximum allowed value is 3153600000 seconds (100 years).|
|Enable “Remember Me”|Website|Defines whether the “Remember Me” checkbox appears on the login and registration pages of the store. Options: <br/>**Yes** - Displays the “Remember Me” checkbox. <br/>**No** - Does not display the “Remember Me” checkbox, and the persistent cookie is used only for customers who already have it.|
|“Remember Me” Default Value|Website|Defines the default state for the “Remember Me” checkbox.|
|Clear Persistence on Log Out|Website|Defines whether the persistent cookie is deleted when a store customer logs out. No matter how Clear Persistence on Log Out is configured, if a customer does not log out, but the session cookie expires, the persistent cookie is still used.|
|Persist Shopping Cart|Website|Defines whether using the persistent cookie gives access to the shopping cart data of the correspondent account. Options: <br/>**Yes** - The shopping cart contents are saved after the session ends. <br/>**No** - The shopping cart contents are not saved after the session ends.|<!--{% if "Default.EE-B2B" contains site.edition %}-->
|Persist Wish List|Website|Determines if the state of customer wish lists is retained when the session ends. Options include: <br/>**Yes** - The wish list contents are saved when the session ends. <br/>**No** - The wish list is not saved when the session ends.|
|Persist Recently Ordered Items|Website|Determines if the state of recently ordered items is retained when the session ends. Options include: <br/>**Yes** - The state of Recently Ordered Items is saved when the session ends. <br/>**No** - The state of Recently Ordered Items is not saved when the session ends.|
|Persist Customer Group Membership and Segmentation|Website|Determines if the state of customers’ group membership and segmentation criteria are retained when the session ends. Options include: <br/>**Yes** - The state of the customer’s group membership and segmentation data is saved when the session ends. <br/>**No** - The state of the customer’s group membership and segmentation data are not saved when the session ends.|<!--{% endif %}-->
