---
title: Authorize.Net
---

Stores > Settings > [Configuration]({{ site.baseurl }}{% link stores/configuration.md %}) > [Sales]({{ site.baseurl }}{% link configuration/sales.md %}) > [Payment Methods]({{ site.baseurl }}{% link configuration/sales/payment-methods.md %}) > Authorize.Net

{:.bs-callout .bs-callout-warning}
**Payment Services Directive Requirements:** <br/>
As of September 14, 2019, European banks might decline payments that do not meet [PSD2]({{ site.baseurl }}{% link stores/compliance-payment-services-directive.md %}) requirements. To comply with PSD2, do one of the following:<br/>- (Recommended) Install and configure the official Authorize.Net payment integration extension from [Magento Marketplace](https://marketplace.magento.com/catalogsearch/result/?q=authorize.net){:target="_blank"}.<br/>- Enable and configure the Authorize.Net payment method in the Magento configuration.<br/>These integrations support 3D Secure 2.0 verification through [CardinalCommerce](https://www.cardinalcommerce.com/products/psd2) and other third-party services.

## Basic Authorize.Net Settings

![]({{ site.baseurl }}{% link images/images/config-sales-payment-methods-authorize-net-basic-settings.png %}){: .zoom}
_Basic Authorize.Net Settings Not Enabled_

![]({{ site.baseurl }}{% link images/images/config-sales-payment-methods-authorize-net-basic-settings-enabled.png %}){: .zoom}
_Basic Authorize.Net Settings Enabled_

|Field|[Scope]({{ site.baseurl }}{% link configuration/scope.md %})|Description|
|--- |--- |--- |
|Enabled|Website|Determines if the Authorize.Net configuration is enabled. To enable the configuration and display additional settings, clear the Use system value checkbox. Then, choose "Yes". Options: Yes / No|
|Title|Store View|A unique label that identifies Authorize.Net in the list of payment methods during checkout.|
|Environment|Website|Indicates the operating mode of your Authorize.Net merchant account. Options: Sandbox / Production (Default) |
|Payment Action|Website|Determines the action taken by Authorize.Net when a payment is authorized. Options: <br/>**Authorize Only** - Funds on the customer's card are authorized, but not transferred from the customer’s account. An order is created in your store Admin. You can later create an invoice and capture the sale. <br/>**Authorize and Capture** - Funds on the customer's card are authorized and captured on the Authorize.Net side, and an order and invoice are created in your store Admin.|
|API Login ID|Website|Your Authorize.Net credentials. Locate your value in your Authorize.Net merchant account. See this Authorize.Net [support article](https://support.authorize.net/s/article/How-do-I-obtain-my-API-Login-ID-and-Transaction-Key) for more information.|
|Transaction Key|Website|Your Authorize.Net credentials. Generate your key value in your Authorize.Net merchant account. See this Authorize.Net [support article](https://support.authorize.net/s/article/How-do-I-obtain-my-API-Login-ID-and-Transaction-Key) for more information.|
|Public Client Key|Website|Your Authorize.Net credentials. Generate your key value in your Authorize.Net merchant account. See this Authorize.Net [support article](https://support.authorize.net/s/article/How-do-I-obtain-my-API-Login-ID-and-Transaction-Key) for more information.|
|Signature Key|Website|Your Authorize.Net credentials. Generate your key value in your Authorize.Net merchant account. See this Authorize.Net [support article](https://support.authorize.net/s/article/How-do-I-obtain-my-API-Login-ID-and-Transaction-Key) for more information.|
|Merchant MD5 (Deprecated)|Website|Authorize.Net has deprecated this field and replaced it with the Signature Key field. If updating from the Authorize.Net Direct Post method to Authorize.Net, this field may auto-populate using your previous settings, but Authorize.Net no longer use this field for transactions. This field will be removed in a later release.|
|Enabled|Website|Determines if Authorize.Net is available to your customers as a payment method at checkout. Options: Yes / No|

## Advanced Authorize.Net Settings

![]({{ site.baseurl }}{% link images/images/config-sales-payment-methods-authorize-net-advanced-settings.png %}){: .zoom}
_Advanced Authorize.Net Settings_

|Field|[Scope]({{ site.baseurl }}{% link configuration/scope.md %})|Description|
|--- |--- |--- |
|Accepted Currency|Website|Must be set to “US Dollar” because this is the only currency that Authorize.Net accepts.|
|Debug|Website|Determines if  messages sent between your store and the Authorize.Net payment system are recorded in a log file. Options: Yes / No <br/><br/>**_Note:_** In accordance with PCI Data Security Standards, credit card information is not recorded in the log file.|
|Email Customer|Website|Determines if Authorize.Net sends a confirmation email when customers complete checkout. This is in addition to the order confirmation email and other email sent from Magento. Options: Yes / No|
|Enable Credit Card Verification Field|Website|Determines if customers are required to enter the Credit Card Verification (CCV) number during checkout. Options: Yes (Default) / No|
|Credit Card Types|Website|Determines the credit cards that are available to customers during checkout. Select each supported card. Options: American Express / Visa / MasterCard / Discover / JCB / Other|
|Payment from Applicable Countries|Website|Determines the range of the applicable country selection. Options: All Allowed Countries / Specific Countries|
|Payment from Specific Countries|Website|Identifies each country from which payment is accepted. Only customers with a billing address in a selected country can make purchases with this payment method.|
|Minimum Order Total|Website|Determines the smallest order total that qualifies to be processed with Authorize.Net.|
|Maximum Order Total|Website|Determines the largest order total that qualifies to be processed with Authorize.Net.|
|Sort Order|Website|A number that determines the order in which Authorize.Net is listed with other payment methods during checkout. Enter 0 for the top of the list.|
