# PJN Data Availability

## Order

### Available Fields

All available fields can be found in the [Shopify API Reference](https://shopify.dev/docs/api/admin-graphql/2024-10/objects/Order).
> **`additionalFees`**
>
>>**`id`**: A globally-unique ID.
>
>> **`name`**: The name of the additional fee.
>
>> **`price`**: The price of the additional fee.
>>>**`presentmentMoney`**: Amount in presentment currency.
>>>>**`amount`**: Decimal money amount.
>
>>>>**`currencyCode`**: Currency of the money.
>
>>>**`shopMoney`**: Amount in presentment currency.
>>>>**`amount`**: Decimal money amount.
>
>>>>**`currencyCode`**: Currency of the money.
>
>> **`taxLines`**: A list of taxes charged on the additional fee.
>>> **`channelLiability`**: Whether the channel that submitted the tax line is liable for remitting. A value of null indicates unknown liability for this tax line.
>
>>> **`priceSet`**: The amount of tax, in shop and presentment currencies, after discounts and before returns.
>
>>> **`rate`**: The proportion of the line item price that the tax represents as a decimal.
>
>>> **`ratePercentage`**: The proportion of the line item price that the tax represents as a percentage.
>
>>> **`source`**: The source of the tax.
>
>>> **`title`**: The name of the tax.
>
>>> **`priceSet`**: The amount of tax, in shop currency, after discounts and before returns. Use priceSet instead.
>
>  **`agreements`**: A list of agreements associated with the order.
>
>> **`arguments`**
>
>>> **`first`**: The first n elements from the paginated list.
>
>>> **`after`**: The elements that come after the specified cursor.
>
>>> **`last`**: The last n elements from the paginated list.
>
>>> **`before`**: The elements that come before the specified cursor.
>
>>> **`reverse`**: Reverse the order of the underlying list.
>
>>> **`query`**: A filter made up of terms, connectives, modifiers, and comparators. You can apply one or more filters to a query. Learn more about Shopify API search syntax.
>
> **`billingAddress`**: The billing address of the customer.
>
>> **`address1`**: The first line of the address. Typically the street address or PO Box number.
>
>> **`address2`**: The second line of the address. Typically the number of the apartment, suite, or unit.
>
>> **`city`**: The city, district, village, or town.
>
>> **`company`**: The company or organisation.
>
>> **`coordinatesValidated`**: Whether address coordinates are valid.
>
>> **`country`**: The name of the country.
>
>> **`countryCodeV2`**: The two-letter code for the country of the address.
>
>> **`firstName`**: The first name of the customer.
>
>> **`formatted`**: The formatted version of the address with ``withName`` or ``withCompany`` as arguments.
>
>> **`id`**: A globally-unique ID.
>
>> **`lastName`**: The last name of the customer.
>
>> **`latitude`**: The latitude coordinate of the customer address.
>
>> **`longitude`**: The longitude coordinate of the customer address.
>
>> **`name`**: The full name of the customer, based on firstName and lastName.
>
>> **`phone`**: The phone number of the customer.
>
>> **`province`**: The region of the address, such as the province, state, or district.
>
>> **`provinceCode`**:The alphanumeric code for the region.
>
>> **`timeZone`**: The time zone of the address.
>
>> **`validationResultSummary`**:Represents the state of validation of a mailing address. For more information, refer to Validating shipping addresses on your orders.
>
>> **`zip`**: The zip or postal code of the address.
>
> **`billingAddressMatchesShippingAddress`**: Whether the billing address matches the shipping address.
>
>**`cancellation`**: Cancellation details for the order.
>
>>**`staffNote`**: Staff provided note for the order cancellation.
>
>**`cancelledAt`**: The date and time when the order was canceled. Returns null if the order wasn't canceled.
>
>**`cancelReason`**: The reason provided when the order was canceled. Returns null if the order wasn't canceled.
>
>**`canMarkAsPaid`**: Whether the order can be manually marked as paid.
>
>**`canNotifyCustomer`**: Whether a customer email exists for the order.
>
>**`capturable`**: Whether payment for the order can be captured.
>
>**`cartDiscountAmountSet`**: The total order-level discount amount, before returns, in shop and presentment currencies.
>
>>**`presentmentMoney`**: Amount in presentment currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>**`channelInformation`**: Details about the channel that created the order.
>
>**`clientIp`**: The IP address of the API client that created the order.
>
>**`closed`**: Whether the order is closed.
>
>**`closedAt`**: The date and time when the order was closed. Returns null if the order isn't closed.
>
>**`confirmationNumber`**: A randomly generated alpha-numeric identifier for the order that may be shown to the customer instead of the sequential order name. For example, "XPAV284CT", "R50KELTJP" or "35PKUN0UJ". This value isn't guaranteed to be unique.
>
>**`confirmed`**: Whether inventory has been reserved for the order.
>
>**`createdAt`**: Date and time when the order was created in Shopify.
>
>**`currencyCode`**: The shop currency when the order was placed.
>
>**`currentCartDiscountAmountSet`**: The current order-level discount amount after all order updates, in shop and presentment currencies.
>
>>**`presentmentMoney`**: Amount in presentment currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>>**`shopMoney`**: Amount in shop currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>**`currentShippingPriceSet`**: The current shipping price after applying refunds and discounts. If the parent order.taxesIncluded field is true, then this price includes taxes. Otherwise, this field is the pre-tax price.
>
>>**`presentmentMoney`**: Amount in presentment currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>>**`shopMoney`**: Amount in shop currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>**`currentSubtotalLineItemsQuantity`**: The sum of the quantities for all line items that contribute to the order's current subtotal price.
>
>**`currentSubtotalPriceSet`**: The sum of the prices for all line items after discounts and returns, in shop and presentment currencies. If taxesIncluded is true, then the subtotal also includes tax.
>
>>**`presentmentMoney`**: Amount in presentment currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>>**`shopMoney`**: Amount in shop currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>**`currentTaxLines`**: A list of all tax lines applied to line items on the order, after returns. Tax line prices represent the total price for all tax lines with the same rate and title.
>
>>**`channelLiable`**: Whether the channel that submitted the tax line is liable for remitting. A value of null indicates unknown liability for this tax line.
>
>>**`priceSet`**: The amount of tax, in shop and presentment currencies, after discounts and before returns.
>
>>**`presentmentMoney`**: Amount in presentment currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>>**`shopMoney`**: Amount in shop currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>>**`rate`**: The proportion of the line item price that the tax represents as a decimal.
>
>>**`ratePercentage`**:The proportion of the line item price that the tax represents as a percentage.
>
>>**`source`**:The source of the tax.
>
>>**`title`**:The name of the tax.
>
>>**`price`**:The amount of tax, in shop currency, after discounts and before returns. Use priceSet instead.
>
>**`currentTotalAdditionalFeesSet`**:The total amount of additional fees after returns, in shop and presentment currencies. Returns null if there are no additional fees for the order.
>
>>**`presentmentMoney`**: Amount in presentment currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>>**`shopMoney`**: Amount in shop currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>**`currentTotalDiscountsSet`**:The total amount discounted on the order after returns, in shop and presentment currencies. This includes both order and line level discounts.
>
>>**`presentmentMoney`**: Amount in presentment currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>>**`shopMoney`**: Amount in shop currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>**`currentTotalDutiesSet`**:The total amount of duties after returns, in shop and presentment currencies. Returns null if duties aren't applicable.
>
>>**`presentmentMoney`**: Amount in presentment currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>>**`shopMoney`**: Amount in shop currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>**`currentTotalPriceSet`**:The total price of the order, after returns, in shop and presentment currencies. This includes taxes and discounts.
>
>>**`presentmentMoney`**: Amount in presentment currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>>**`shopMoney`**: Amount in shop currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>**`currentTotalTaxSet`**:The sum of the prices of all tax lines applied to line items on the order, after returns, in shop and presentment currencies.
>
>>**`presentmentMoney`**: Amount in presentment currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>>**`shopMoney`**: Amount in shop currency.
>
>>>**`amount`**: Decimal money amount.
>
>>>**`currencyCode`**: Currency of the money.
>
>**`currentTotalWeight`**:The total weight of the order after returns, in grams.
>
>**`customAttributes`**:A list of additional merchant-facing details that have been added to the order. For example, whether an order is a customer's first.
>
>>**`key`**:The key or name of the attribute. For example, "customersFirstOrder".
>
>>**`value`**:The value of the attribute. For example, "true".
>
>**`customer`**:The customer that placed the order.
>
>>**`addresses`**:A list of addresses associated with the customer.
>
>>>**`fields`**
>
>>>>**`address1`**
>
>>>>**`address2`**: The second line of the address. Typically the number of the apartment, suite, or unit.
>
>>>>**`city`**:The name of the city, district, village, or town.
>
>>>>**`company`**:The name of the customer's company or organization.
>
>>>>**`coordinatesValidated`**:Whether the address coordinates are valid.
>
>>>>**`country`**:The name of the country.
>
>>>>**`countryCodeV2`**:The two-letter code for the country of the address. For example, US.
>
>>>>**`firstName`**:The first name of the customer.
>
>>>>**`formatted`**:A formatted version of the address, customized by the provided arguments.
>
>>>>>**`withName`**:Whether to include the customer's name in the formatted address.
>
>>>>>**`withCompany`**:Whether to include the customer's company in the formatted address.
>
>>>>**`formattedArea`**:A comma-separated list of the values for city, province, and country.
>
>>>>**`id`**:A globally-unique ID.
>
>>>>**`lastName`**:The last name of the customer.
>
>>>>**`latitude`**:The latitude coordinate of the customer address.
>
>>>>**`longitude`**:The longitude coordinate of the customer address.
>
>>>>**`name`**:The full name of the customer, based on firstName and lastName.
>
>>>>**`phone`**:A unique phone number for the customer.
>
>>>>**`province`**:The region of the address, such as the province, state, or district.
>
>>>>**`provinceCode`**:The alphanumeric code for the region.For example, ON.
>
>>>>**`timeZone`**:The time zone of the address.
>
>>>>**`validationResultSummary`**:Represents the state of validation of a mailing address. For more information, refer to Validating shipping addresses on your orders.
>
>>>>**`zip`**:The zip or postal code of the address.
>
>>>>**`countryCode`**:The two-letter code for the country of the address.
>
>>**`addressesV2`**:A list of addresses associated with the customer.
>
>**`amountSpent`**:The total amount that the customer has spent on orders in their lifetime.
>
>>**`amount`**:Decimal money amount.
>
>>**`currencyCode`**:Currency of the money.
>
>**`canDelete`**:Whether the merchant can delete the customer from their store. A customer can be deleted from a store only if they haven't yet made an order. After a customer makes an order, they can't be deleted from a store.
>
>**`companyContactProfiles`**:A list of the customer's company contact profiles.
>
>>**`company`**:The company to which the contact belongs.
>
>>**`createdAt`**:The date and time (ISO 8601 format) at which the company contact was created at Shopify.
>
>>**`customer`**:The customer associated to this contact.
>
>>**`draftOrders`**:The list of draft orders for the company contact.
>
>>**`id`**:A globally-unique ID.
>
>>**`isMainContact`**:Whether the contact is the main contact of the company.
>
>>**`lifetimeDuration`**:The lifetime duration of the company contact, since its creation date on Shopify. Examples: 1 year, 2 months, 3 days.
>
>>**`locale`**:The company contact's locale (language).
>
>>**`orders`**:The list of orders for the company contact.
>
>>**`roleAssignments`**:The list of roles assigned to this company contact.
>
>>**`title`**:The company contact's job title.
>
>>**`updatedAt`**:The date and time (ISO 8601 format) at which the company contact was last updated.
>
>>**`createdAt`**:The date and time when the customer was added to the store.
>
>>**`dataSaleOptOut`**:Whether the customer has opted out of having their data sold.
>
>>**`defaultAddress`**:The default address associated with the customer.
>
>>**`displayName`**:The full name of the customer, based on the values for first_name and last_name. If the first_name and last_name are not available, then this falls back to the customer's email address, and if that is not available, the customer's phone number.
>
>>**`email`**:The customer's email address.
>
>>**`emailMarketingConsent`**:The current email marketing state for the customer. If the customer doesn't have an email address, then this property is null.
>
>>>**`consentUpdatedAt`**:The date and time at which the customer consented to receive marketing material by email. The customer's consent state reflects the consent record with the most recent consent_updated_at date. If no date is provided, then the date and time at which the consent information was sent is used.
>
>>>**`marketingOptInLevel`**:The marketing subscription opt-in level, as described by the M3AAWG best practices guidelines, that the customer gave when they consented to receive marketing material by email.
>
>>>**`marketingState`**:The current email marketing state for the customer.
>
>>**`events`**:A list of events associated with the customer.
>
>>**`firstName`**:The customer's first name.
>
>>**`id`**:A globally-unique ID.
>
>>**`image`**:A globally-unique I
>
>>**`lastName`**:The customer's last name.
>
>>**`lastOrder`**:The customer's last order.
>
>>**`legacyResourceId`**:The ID of the corresponding resource in the REST Admin API.
>
>>**`lifetimeDuration`**:The amount of time since the customer was first added to the store.
>
>>**`locale`**:The customer's locale.
>
>>**`market`**:The market that includes the customer’s default address.
>
>>**`mergeable`**:Whether the customer can be merged with another customer.
>
>>**`metafield`**:A custom field, including its namespace and key, that's associated with a Shopify resource for the purposes of adding and storing additional information.
>
>>**`metafieldS`**:A list of custom fields that a merchant associates with a Shopify resource.
>
>>**`multipassIdentifier`**:A unique identifier for the customer that's used with Multipass login.
>
>>**`note`**:A note about the customer.
>
>>**`numberOfOrders`**:The number of orders that the customer has made at the store in their lifetime.
>
>>**`orders`**:A list of the customer's orders.
>
>>**`paymentMethods`**:A list of the customer's payment methods.
>
>>**`phone`**:The customer's phone number.
>
>>**`productSubscriberStatus`**:Possible subscriber states of a customer defined by their subscription contracts.
>
>>**`smsMarketingConsent`**:The current SMS marketing state for the customer's phone number.If the customer does not have a phone number, then this property is null
>
>>**`state`**:The state of the customer's account with the shop.Please note that this only meaningful when Classic Customer Accounts is active.
>
>>**`statistics`**:The statistics for a given customer.
>
>>**`storeCreditAccounts`**:Returns a list of store credit accounts that belong to the owner resource.
>
>>**`subscriptionContracts`**:A list of the customer's subscription contracts.
>
>>**`tags`**:A comma separated list of tags that have been added to the customer.
>
>>**`taxExempt`**:Whether the customer is exempt from being charged taxes on their orders.
>
>>**`taxExemptions`**:The list of tax exemptions applied to the customer.
>
>>**`unsubscribeUrl`**:The URL to unsubscribe the customer from the mailing list.
>
>>**`updatedAt`**:The date and time when the customer was last updated.
>
>>**`validEmailAddress`**:Whether the email address is formatted correctly.Returns true when the email is formatted correctly and belongs to an existing domain. This doesn't guarantee that the email address actually exists.
>
>>**`verifiedEmail`**:Whether the customer has verified their email address. Defaults to true if the customer is created through the Shopify admin or API.
>
>**`customerAcceptsMarketing`**:Whether the customer agreed to receive marketing materials.
>
>**`customerJourneySummary`**:The customer's visits and interactions with the online store before placing the order.
>
>>**`customerOrderIndex`**:The position of the current order within the customer's order history. Test orders aren't included.
>
>>**`daysToConversion`**:The number of days between the first session and the order creation date. The first session represents the first session since the last order, or the first session within the 30 day attribution window, if more than 30 days have passed since the last order.
>
>>**`firstVisit`**:The customer's first session going into the shop.
>
>>>**`id`**:A globally-unique ID.
>
>>>**`landingPage`**:URL of the first page the customer landed on for the session.
>
>>>**`landingPageHtml`**:Landing page information with URL linked in HTML. For example, the first page the customer visited was store.myshopify.com/products/1.
>
>>>**`marketingEvent`**:MarketingEvent Represent actions taken by an app, on behalf of a merchant, to market Shopify resources such as products, collections, and discounts.
>
>>>**`occurredAt`**:The date and time when the customer's session occurred.
>
>>>**`referralCode`**:Marketing referral code from the link that the customer clicked to visit the store. Supports the following URL attributes: ref, source, or r. For example, if the URL is myshopifystore.com/products/slide?ref=j2tj1tn2, then this value is j2tj1tn2.
>
>>>**`referralInfoHtml`**:Referral information with URLs linked in HTML.
>
>>>**`referrerUrl`**:Webpage where the customer clicked a link that sent them to the online store. For example, https://randomblog.com/page1 or android-app://com.google.android.gm.
>
>>>**`source`**:Source from which the customer visited the store, such as a platform (Facebook, Google), email, direct, a website domain, QR code, or unknown.
>
>>>**`sourceDescription`**:Describes the source explicitly for first or last session.
>
>>>**`sourceType`**:Type of marketing tactic.
>
>>>**`utmParameters`**:A set of UTM parameters gathered from the URL parameters of the referrer.
>
>>**`lastVisit`**:The last session before an order is made.
>
>>>**`id`**:A globally-unique ID.
>
>>>**`landingPage`**:URL of the first page the customer landed on for the session.
>
>>>**`landingPageHtml`**:Landing page information with URL linked in HTML. For example, the first page the customer visited was store.myshopify.com/products/1.
>
>>>**`marketingEvent`**:MarketingEvent Represent actions taken by an app, on behalf of a merchant, to market Shopify resources such as products, collections, and discounts.
>
>>>**`occurredAt`**:The date and time when the customer's session occurred.
>
>>>**`referralCode`**:Marketing referral code from the link that the customer clicked to visit the store. Supports the following URL attributes: ref, source, or r. For example, if the URL is myshopifystore.com/products/slide?ref=j2tj1tn2, then this value is j2tj1tn2.
>
>>>**`referralInfoHtml`**:Referral information with URLs linked in HTML.
>
>>>**`referrerUrl`**:Webpage where the customer clicked a link that sent them to the online store. For example, https://randomblog.com/page1 or android-app://com.google.android.gm.
>
>>>**`source`**:Source from which the customer visited the store, such as a platform (Facebook, Google), email, direct, a website domain, QR code, or unknown.
>
>>>**`sourceDescription`**:Describes the source explicitly for first or last session.
>
>>>**`sourceType`**:Type of marketing tactic.
>
>>>**`utmParameters`**:A set of UTM parameters gathered from the URL parameters of the referrer.
>
>>**`moments`**:The events preceding a customer's order, such as shop sessions.
>
>>**`momentsCount`**:The total number of customer moments associated with this order. Returns null if the order is still in the process of being attributed.
>
>>**`ready`**:Whether the attributed sessions for the order have been created yet.
>
>**`customerLocale`**:A two-letter or three-letter language code, optionally followed by a region modifier.
>
>**`discountApplications`**:A list of discounts that are applied to the order, not including order edits and refunds.
>
>**`discountCode`**:The discount code used for the order.
>
>**`discountCodes`**:The discount codes used for the order.
>
>**`displayAddress`**:The primary address of the customer. Returns null if neither the shipping address nor the billing address was provided.
>
>**`displayFinancialStatus`**:The financial status of the order that can be shown to the merchant. This field doesn't capture all the details of an order's financial state. It should only be used for display summary purposes.
>
>**`displayFulfillmentStatus`**:The fulfillment status for the order that can be shown to the merchant. This field does not capture all the details of an order's fulfillment state. It should only be used for display summary purposes. For a more granular view of the fulfillment status, refer to the FulfillmentOrder object.
>
>**`disputes`**:A list of the disputes associated with the order.
>
>>**`id`**:A globally-unique ID.
>
>>**`initiatedAs`**:The type that the dispute was initiated as.
>
>>**`status`**:The current status of the dispute.
>
>**`dutiesIncluded`**:Whether duties are included in the subtotal price of the order.
>
>**`edited`**:Whether the order has had any edits applied.
>
>**`email`**:The email address associated with the customer.
>
>**`estimatedTaxes`**:Whether taxes on the order are estimated. This field returns false when taxes on the order are finalized and aren't subject to any changes.
>
>**`events`**:A list of events associated with the order.
>
>**`fulfillable`**:Whether there are line items that can be fulfilled. This field returns false when the order has no fulfillable line items. For a more granular view of the fulfillment status, refer to the FulfillmentOrder object.
>
>**`fulfillmentOrders`**:A list of fulfillment orders for a specific order.FulfillmentOrder API access scopes govern which fulfillments orders are returned. An API client will only receive a subset of the fulfillment orders which belong to an order if they don't have the necessary access scopes to view all of the fulfillment orders. In the case that an API client does not have the access scopes necessary to view any of the fulfillment orders that belong to an order, an empty array will be returned.
>
>**`fulfillments`**:List of shipments for the order.
>
>**`fulfillmentsCount`**:The count of fulfillments including the cancelled fulfillments.
>
>**`fullyPaid`**:Whether the order has been paid in full.
>
>**`hasTimelineComment`**:Whether the merchant added a timeline comment to the order.
>
>**`id`**:A globally-unique ID.
>
>**`legacyResourceId`**:The ID of the corresponding resource in the REST Admin API.
>
>**`lineItems`**:A list of the order's line items.
>
>**`localizationExtensions`**:List of localization extensions for the resource.
>
>**`merchantBusinessEntity`**:The merchant's business entity associated with the order.
>
>**`merchantEditable`**:Whether the order can be edited by the merchant. For example, canceled orders can’t be edited.
>
>**`merchantEditableErrors`**:A list of reasons why the order can't be edited. For example, "Canceled orders can't be edited".
>
>**`merchantOfRecordApp`**:The application acting as the Merchant of Record for the order.
>
>**`metafield`**:A custom field, including its namespace and key, that's associated with a Shopify resource for the purposes of adding and storing additional information.
>
>>**`namespace`**:A list of custom fields that a merchant associates with a Shopify resource.
>
>>**`keys`**:List of keys of metafields in the format namespace.key, will be returned in the same format.

>
>**`metafields`**:A list of custom fields that a merchant associates with a Shopify resource.
>
>>**`namespace`**:A list of custom fields that a merchant associates with a Shopify resource.
>
>>**`keys`**:List of keys of metafields in the format namespace.key, will be returned in the same format.
>
>**`name`**:The unique identifier for the order that appears on the order page in the Shopify admin and the Order status page. For example, "#1001", "EN1001", or "1001-A". This value isn't unique across multiple stores.
>
>**`netPaymentSet`**:The net payment for the order, based on the total amount received minus the total amount refunded, in shop and presentment currencies.
>
>**`nonFulfillableLineItems`**:A list of line items that can't be fulfilled. For example, tips and fully refunded line items can't be fulfilled. For a more granular view of the fulfillment status, refer to the FulfillmentOrder object.
>
>**`note`**:The contents of the note associated with the order.
>
>**`originalTotalAdditionalFeesSet`**:The total amount of additional fees at the time of order creation, in shop and presentment currencies. Returns null if additional fees aren't applicable.
>
>**`originalTotalDutiesSet`**:The total amount of duties at the time of order creation, in shop and presentment currencies. Returns null if duties aren't applicable.
>
>**`originalTotalPriceSet`**:The total price of the order at the time of order creation, in shop and presentment currencies.
>
>**`paymentCollectionDetails`**:The payment collection details for the order.
>
>**`paymentGatewayNames`**:A list of the names of all payment gateways used for the order. For example, "Shopify Payments" and "Cash on Delivery (COD)".
>
>**`paymentTerms`**:The payment terms associated with the order.
>
>**`phone`**:The phone number associated with the customer.
>
>**`poNumber`**:The PO number associated with the order.
>
>**`presentmentCurrencyCode`**:The payment CurrencyCode of the customer for the order.
>
>**`processedAt`**:The date and time when the order was processed. This date and time might not match the date and time when the order was created.
>
>**`publication`**:The publication that the order was created from.
>
>**`purchasingEntity`**:The purchasing entity for the order.
>
>**`refundable`**:Whether the order can be refunded.
>
>**`refundDiscrepancySet`**:The difference between the suggested and actual refund amount of all refunds that have been applied to the order. A positive value indicates a difference in the merchant's favor, and a negative value indicates a difference in the customer's favor.
>
>**`refunds`**:A list of refunds that have been applied to the order.
>
>**`registeredSourceUrl`**:The URL of the source that the order originated from, if found in the domain registry.
>
>**`requiresShipping`**:Whether the order has shipping lines or at least one line item on the order that requires shipping.
>
>**`restockable`**:Whether any line item on the order can be restocked.
>
>**`retailLocation`**:The physical location where a retail order is created or completed, except for draft POS orders completed via the “mark as paid” flow in Admin, which return null.
>
>**`returns`**:A list of returns for the order.
>
>**`returnStatus`**:The order's aggregated return status for display purposes.
>
>**`risk`**:The risk characteristics for the order.
>
>**`shippingAddress`**:The mailing address of the customer.
>
>**`shippingLine`**:A summary of all shipping costs on the order.
>
>**`shippingLines`**:A list of the order's shipping lines.
>
>**`shopifyProtect`**:The Shopify Protect details for the order. If Shopify Protect is disabled for the shop, then this will be null.
>
>**`sourceIdentifier`**:A unique POS or third party order identifier. For example, "1234-12-1000" or "111-98567-54". The receipt_number field is derived from this value for POS orders.
>
>**`sourceName`**:The name of the source associated with the order.
>
>**`staffMember`**:The staff member associated with the order.
>
>**`statusPageUrl`**:The URL where the customer can check the order's current status.
>
>**`subtotalLineItemsQuantity`**:The sum of the quantities for all line items that contribute to the order's subtotal price.
>
>**`subtotalPriceSet`**:The sum of the prices for all line items after discounts and before returns, in shop and presentment currencies. If taxesIncluded is true, then the subtotal also includes tax.
>
>**`suggestedRefund`**:A suggested refund for the order.
>
>**`tags`**:A comma separated list of tags associated with the order. Updating tags overwrites any existing tags that were previously added to the order. To add new tags without overwriting existing tags, use the tagsAdd mutation.
>
>**`taxesIncluded`**:Whether taxes are included in the subtotal price of the order.
>
>**`taxExempt`**:Whether taxes are exempt on the order.
>
>**`taxLines`**:A list of all tax lines applied to line items on the order, before returns. Tax line prices represent the total price for all tax lines with the same rate and title.
>
>**`test`**:Whether the order is a test. Test orders are made using the Shopify Bogus Gateway or a payment provider with test mode enabled. A test order can't be converted into a real order and vice versa.
>
>**`totalCapturableSet`**:The authorized amount that's uncaptured or undercaptured, in shop and presentment currencies. This amount isn't adjusted for returns.
>
>**`totalCashRoundingAdjustment`**:The total rounding adjustment applied to payments or refunds for an Order involving cash payments. Applies to some countries where cash transactions are rounded to the nearest currency denomination.
>
>**`totalDiscountsSet`**:The total amount discounted on the order before returns, in shop and presentment currencies. This includes both order and line level discounts.
>
>**`totalOutstandingSet`**:The total amount not yet transacted for the order, in shop and presentment currencies. A positive value indicates a difference in the merchant's favor (payment from customer to merchant) and a negative value indicates a difference in the customer's favor (refund from merchant to customer).
>
>**`totalPriceSet`**:The total price of the order, before returns, in shop and presentment currencies. This includes taxes and discounts.
>
>**`totalReceivedSet`**:The total amount received from the customer before returns, in shop and presentment currencies.
>
>**`totalRefundedSet`**:The total amount that was refunded, in shop and presentment currencies.
>
>**`totalRefundedShippingSet`**:The total amount of shipping that was refunded, in shop and presentment currencies.
>
>**`totalShippingPriceSet`**:The total shipping amount before discounts and returns, in shop and presentment currencies.
>
>**`totalTaxSet`**:The total tax amount before returns, in shop and presentment currencies.
>
>**`totalTipReceivedSet`**:The sum of all tip amounts for the order, in shop and presentment currencies.
>
>**`totalWeight`**:The total weight of the order before returns, in grams.
>
>**`transactions`**:A list of transactions associated with the order.
>
>**`transactionsCount`**:The number of transactions associated with the order.
>
>**`unpaid`**:Whether no payments have been made for the order.
>
>**`updatedAt`**:The date and time when the order was modified last.


















































































































































### GraphQL Query Example To Calculate Refund

```
query SuggestedRefund($id: ID!, $refundLineItems: [RefundLineItemInput!]) {
  order(id: $id) {
    id
    suggestedRefund(refundLineItems: $refundLineItems) {
      subtotalSet {
        shopMoney {
          amount
          currencyCode
        }
        presentmentMoney {
          amount
          currencyCode
        }
      }
      refundLineItems {
        lineItem {
          id
        }
        quantity
      }
    }
  }
}

```

### Input variables Example

```
{
  "id": "gid://shopify/Order/469306983",
  "refundLineItems": [
    {
      "lineItemId": "gid://shopify/LineItem/983004162",
      "quantity": 1
    }
  ]
}


```

### Response Example

```
{
  "order": {
    "id": "gid://shopify/Order/469306983",
    "suggestedRefund": {
      "subtotalSet": {
        "shopMoney": {
          "amount": "8.26",
          "currencyCode": "USD"
        },
        "presentmentMoney": {
          "amount": "7.0",
          "currencyCode": "EUR"
        }
      },
      "refundLineItems": [
        {
          "lineItem": {
            "id": "gid://shopify/LineItem/983004162"
          },
          "quantity": 1
        }
      ]
    }
  }
}

```





## Customer

### Available Fields
All available fields can be found in the [Shopify API Reference](https://shopify.dev/docs/api/admin-graphql/2024-10/queries/customer).

> `addresses`
>
>> `address1`: first line of the address
>
>> `address2`: second line of the address
>
>> `city`: city, district, village, town
>
>> `company`: company or organisation
>
>> `coordinatesValidated`: whether address coordinates are valid
>
>> `country`
>
>> `countryCodeV2`
>
>> `firstName`
>
>> `formatted`: formatted version of the address with ``withName`` or ``withCompany`` as arguments
>
>> `formattedArea`: comma-seperated value list for address
>
>> `id`
>
>> `lastName`
>
>> `latitude`
>
>> `longitude`
>
>> `name`: full name
>
>> `phone`: unique phone number
>
>> `province`: province, state, district
>
>> `provinceCode`: alphanumeric code for the region
>
>> `timeZone`
>
>> `validationResultSummary`: state of validation of a mailing address
>
>> `zip`: zip or postal code

> `addressesV2`
>
> `amountSpent`: lifetime order amount spent
>
> `canDelete`: whether or not a customer can be deleted
>
> `companyContactProfiles`
>
>> `company`
>
>> `createdAt`: date and time the company contact was created
>
>> `customer`
>
>> `draftOrders`: list of draft orders for the company contact
>
>> `id`
>
>> `isMainContact`
>
>> `lifetimeDuration`
>
>> `locale`: company contact's locale (language)
>
>> `orders`: list of orders for the customer contact
>
>> `roleAssignments`: roles assigned to company contact
>
>> `title`: job title
>
>> `updatedAt`
>
> `createdAt`: date and time when customer was added to the store
>
> `dataSaleOptOut`: whether customer has opted out of having their data sold
>
> `defaultAddress`
>
> `displayName`: full name based on first and last name
>
> `email`
>
> `emailMarketingConsent`
>
>> `consentUpdatedAt`: date and time the customer consented to receive marketing materials
>
>> `marketingOptInLevel`
>
>> `marketingState`
>
> `events`: list of events associated with the customer
>
> `firstName`
>
> `id`
>
> `image`
>
>> `altText`
>
>> `height`
>
>> `id`
>
>> `metafield`
>
>> `metafields`: list of metafields
>
>> `url`
>
>> `width`
>
> `lastName`
>
> `lastOrder`
>
> `legacyResourceId`
>
> `lifetimeDuration`
>
> `locale`
>
> `market`: the market that includes the customer's default address
>
>> `catalogs`
>
>> `catalogsCount`
>
>> `currencySettings`
>
>> `enabled`
>
>> `handle`
>
>> `id`
>
>> `metafield`
>
>> `metafields`
>
>> `name`: name of the market
>
>> `primary`: true or false
>
>> `regions`: the regions that make up the market
>
>> `webPresence`: the web presence that defines its SEO strategy
>
>> `priceList`: price list, specifies percentage-based price adjustment and fixed-price overrides for specific variants
>
> `mergeable`: whether a customer can be merged with another
>
> `metafield`: A custom field, including its namespace and key, that's associated with a Shopify resource for the purposes of adding and storing additional information.
>
> `metafields`: list
>
> `multipassIdentifier`
>
> `note`
>
> `numberOfOrders`
>
> `orders`: list of past orders
>
> `paymentMethods`
>
> `phone`
>
> `productSubscriberStatus`
>
>> ACTIVE, CANCELLED, EXPIRED, FAILED, NEVER SUBSCRIBED, PAUSED
>
> `smsMarketingConsent`: SMS marketing state for the customers number
>
>> `consentCollectedFrom`: the source from where the consent was collected
>
>>> `OTHER`
>
>>> `SHOPIFY`
>
>> `consentUpdatedAt`: date and time
>
>> `marketingOptInLevel`
>
>>> `CONFIRMED_OPT_IN`
>
>>> `SINGLE_OPT_IN`
>
>>> `UNKNOWN`
>
>> `marketingState`
>
>>> `NOT_SUBSCRIBED`
>
>>> `PENDING`
>
>>> `REDACTED`
>
>>> `SUBSCRIBED`
>
>>> `UNSUBSCRIBED`
>
> `state`: the state of the customers account with the shop
>
>> `DECLINED`
>
>> `DISABLED`
>
>> `ENABLED`
>
>> `INVITED`
>
> `statistics`
>
>> `predictedeSpendTier`
>
>>> `HIGH`
>
>>> `LOW`
>
>>> `MEDIUM`
>
> `storeCreditAccounts`
>
> `subscriptionContracts`
>
> `tags`: commas seperated list of tags added to the customer
>
> `taxEmxempt`
>
> `taxExemptions`: list of tax exemptions applied to the customer
>
> `unsubscribeURL`: URL to unsusbcribe customer from mailing list
>
> `updatedAt`: Date and time
>
> `validEmailAddress`: whether the email address is formatted correctly
>
> `verifiedEmail`: whether the customer has verified their email address

### GraphQL Query Example

```
query {
  customer(id: "gid://shopify/Customer/544365967") {
    id
    firstName
    lastName
    email
    phone
    numberOfOrders
    amountSpent {
      amount
      currencyCode
    }
    createdAt
    updatedAt
    note
    verifiedEmail
    validEmailAddress
    tags
    lifetimeDuration
    defaultAddress {
      formattedArea
      address1
    }
    addresses {
      address1
    }
    image {
      src
    }
    canDelete
  }
}

```
### Response Example

```

{
  "customer": {
    "id": "gid://shopify/Customer/544365967",
    "firstName": "Bob",
    "lastName": "Bobsen",
    "email": "bob@example.com",
    "phone": "+13125551212",
    "numberOfOrders": "25",
    "amountSpent": {
      "amount": "8305.6",
      "currencyCode": "USD"
    },
    "createdAt": "2005-06-15T15:57:11Z",
    "updatedAt": "2005-06-16T15:57:11Z",
    "note": null,
    "verifiedEmail": true,
    "validEmailAddress": true,
    "tags": [
      "Bob",
      "Canadian",
      "Léon",
      "Noël"
    ],
    "lifetimeDuration": "over 19 years",
    "defaultAddress": {
      "formattedArea": "Ottawa ON, Canada",
      "address1": "123 Amoebobacterieae St"
    },
    "addresses": [
      {
        "address1": "123 Amoebobacterieae St"
      }
    ],
    "image": {
      "src": "https://cdn.shopify.com/proxy/d02a582792c73c48b4b62a95f42bcbf6eff91c5d232efb2057ca4c41005e4728/www.gravatar.com/avatar/4b9bb80620f03eb3719e0a061c14283d.jpg?s=2048&d=https%3A%2F%2Fcdn.shopify.com%2Fshopifycloud%2Fshopify%2Fassets%2Fadmin%2Fcustomers%2Fpolaris%2Favatar-2-a0ee6e3fb3ae515b66b68388b265e5bd1e90646c4c72d59170518f45351e668b.png"
    },
    "canDelete": false
  }
}

```
