Variables for templates
=======================

There is the list of all variables which are using in templates. So you can use them in your custom templates.

####Basic system values:
- *details*
- *summary* {{ dump(loader.values) }} *</summary<br>*
- *p markdown="1"*


##### result will be array of company fields:

     object(models\common\finance\TemplateValues)#226 (30) {
     ["id"]=> string(2) "13"
     ["invoice_template_id"]=> string(1) "5"
     ["request_template_id"]=> string(2) "14"
     ["receipt_template_id"]=> string(2) "34"
     ["reminder_mail_template_id"]=> string(2) "15"
     ["reminder_sms_template_id"]=> string(2) "16"
     ["company_name"]=> string(33) "Private Company Internet Ltd."
     ["street_1"]=> string(47) "56, Adamause str."
     ["street_2"]=> string(0) ""
     ["zip"]=> string(6) "568749"
     ["city"]=> string(8) "Yamayka"
     ["country"]=> string(5) "Gonduras"
     ["email"]=> string(20) "office@privatecompany.com"
     ["phone"]=> string(14) "8 500 600 8526"
     ["company_id"]=> string(21) "K683621TP2398723321"
     ["company_vat"]=> string(0) ""
     ["vat_percent"]=> string(7) "20.0000"
     ["bank_account"]=> string(0) ""
     ["bank_name"]=> string(0) ""
     ["bank_id"]=> string(0) ""
     ["bank_address"]=> string(0) ""
     ["splynx_url"]=> string(44) "https://privatecompany/admin/login"
     ["partner_percent"]=> string(4) "0.00"
     ["deleted"]=> NULL
     ["_relations":"db\Record":private]=> array(0) { }
     ["connected_models":"db\Record":private]=> NULL
     ["_oldAttributes":protected]=> array(23) {
             some old attributes ...
             }
     ["_errors":"base\Model":private]=> NULL
     ["_additionalAttributes":protected]=> array(0) { }
     ["_isAdditionalAttributesLoaded":protected]=> bool(false)
     }
</p>
</details>

####Customer's information:
details<br>
summary {{ dump(customer) }}</summary<br>
p markdown="1"

##### result will be array of customer fields:

     array(38) {
     ["id"]=> string(1) "4"
     ["billing_type"]=> string(7) "prepaid"
     ["partner_id"]=> string(2) "13"
     ["location_id"]=> string(1) "3"
     ["added_by"]=> string(5) "admin"
     ["added_by_id"]=> string(1) "1"
     ["login"]=> string(11) "qwerty"
     ["category"]=> string(6) "person"
     ["password"]=> string(11) "ZaXsCdVfBg"
     ["name"]=> string(12) "Qwert Ytrewq"
     ["email"]=> string(19) "qwerty@gmail.com"
     ["phone"]=> string(10) "132456789"
     ["street_1"]=> string(57) "Long Island str., 526/4"
     ["zip_code"]=> string(0) "48567"
     ["city"]=> string(0) "Malibu"
     ["status"]=> string(6) "active"
     ["date_add"]=> string(10) "2016-05-21"
     ["last_online"]=> string(19) "2017-06-01 11:41:01"
     ["last_update"]=> string(19) "2017-05-01 14:10:50"
     ["internet_tariffs"]=> NULL
     ["voice_tariffs"]=> NULL
     ["custom_tariffs"]=> NULL
     ["services_internet_router_id"]=> NULL
     ["services_internet_sector_id"]=> NULL
     ["services_internet_login"]=> NULL
     ["services_internet_ipv4"]=> NULL
     ["services_internet_ipv4_route"]=> NULL
     ["services_internet_mac"]=> NULL
     ["services_voice_phone"]=> NULL
     ["services_voice_voice_device_id"]=> NULL
     ["services_internet_start_date"]=> NULL
     ["services_internet_end_date"]=> NULL
     ["services_voice_start_date"]=> NULL
     ["services_voice_end_date"]=> NULL
     ["services_custom_start_date"]=> NULL
     ["services_custom_end_date"]=> NULL
     ["deleted"]=> string(1) "0"
     ["additional_attributes"]=> array(10) {
             ["some_additional_field"]=> string(0) "some additional field"
             }
     }
</p>
</details>

####General information:
details<br>
summary>{{ dump(loader.info) }}</summary<br>
p markdown="1">

##### result will be array of customer's information fields:

     object(models\common\customers\CustomerInfo)#226 (12) {
     ["customer_id"]=> string(1) "4"
     ["birthday"]=> string(0) ""
     ["passport"]=> string(0) ""
     ["company_id"]=> string(0) ""
     ["vat_id"]=> string(0) ""
     ["deleted"]=> NULL
     ["_relations":"db\Record":private]=> array(0) { }
     ["connected_models":"db\Record":private]=> NULL
     ["_oldAttributes":protected]=> array(5) {
             some old attributes ...
             }
     ["_errors":"base\Model":private]=> NULL
     ["_additionalAttributes":protected]=> array(0) { }
     ["_isAdditionalAttributesLoaded":protected]=> bool(false)
     }
</p>


####Billing information:
details<br>
summary>{{ dump(loader.billing) }}</summary<br>
p markdown="1">

##### result will be array of billing fields:

     object(models\common\customers\CustomerBilling)#226 (36) {
     ["customer_id"]=> string(1) "4"
     ["enabled"]=> string(1) "1"
     ["type"]=> string(1) "1"
     ["deposit"]=> string(8) "758.0000"
     ["billing_date"]=> string(1) "1"
     ["billing_due"]=> string(2) "15"
     ["grace_period"]=> string(2) "10"
     ["make_invoices"]=> string(1) "1"
     ["auto_pay_invoices_from_deposit"]=> string(0) ""
     ["payment_method"]=> string(1) "1"
     ["min_balance"]=> string(6) "0.0000"
     ["request_auto_enable"]=> string(0) ""
     ["request_auto_day"]=> string(1) "1"
     ["request_auto_period"]=> string(1) "0"
     ["reminder_enable"]=> string(1) "1"
     ["reminder_day_1"]=> string(1) "2"
     ["reminder_day_2"]=> string(1) "8"
     ["reminder_day_3"]=> string(2) "20"
     ["reminder_payment"]=> string(0) ""
     ["reminder_payment_value"]=> string(6) "0.0000"
     ["reminder_payment_comment"]=> string(0) ""
     ["reminder_type"]=> string(1) "0"
     ["billing_person"]=> string(0) ""
     ["billing_street_1"]=> string(0) ""
     ["billing_zip_code"]=> string(0) ""
     ["billing_city"]=> string(0) ""
     ["request_auto_type"]=> string(1) "1"
     ["request_auto_next"]=> string(10) "0000-00-00"
     ["partner_id"]=> NULL ["deleted"]=> string(1) "0"
     ["_relations":"db\Record":private]=> array(0) { }
     ["connected_models":"db\Record":private]=> NULL
     ["_oldAttributes":protected]=> array(29) {
             some old attributes ...
             }
     ["_errors":"base\Model":private]=> NULL
     ["_additionalAttributes":protected]=> array(0) { }
     ["_isAdditionalAttributesLoaded":protected]=> bool(false)
     }
</p>


####Partner:
details<br>
summary>{{ dump(loader.partner) }}</summary<br>
p markdown="1">

##### result will be array of partner fields:

     object(models\admin\administration\Partners)#226 (11) {
     ["id"]=> string(2) "13"
     ["name"]=> string(14) "Partner West"
     ["ips_to_remove":"db\ActiveTable":private]=> array(0) { }
     ["relatedItems":protected]=> array(0) { }
     ["deleted"]=> string(1) "0"
     ["_relations":"db\Record":private]=> array(0) { }
     ["connected_models":"db\Record":private]=> NULL
     ["_oldAttributes":protected]=> array(3) {
             ["id"]=> string(2) "13"
             ["name"]=> string(14) "Partner West"
             ["deleted"]=> string(1) "0"
             }
     ["_errors":"base\Model":private]=> NULL
     ["_additionalAttributes":protected]=> array(1) {
             ["code"]=> string(4) "EUR"
             }
     ["_isAdditionalAttributesLoaded":protected]=> bool(true) }
</p>


####Transactions:
details<br>
summary>{{ dump(loader.transactions) }}</summary<br>
p markdown="1">

##### result will be array of transactions fields:

     array(3) {
     [158]=> object(models\common\finance\Transactions)#226 (32) {
             ["id"]=> string(4) "158"
             ["customer_id"]=> string(1) "4"
             ["type"]=> string(6) "credit"
             ["quantity"]=> string(1) "1"
             ["unit"]=> string(0) ""
             ["price"]=> string(9) "1033.8500"
             ["tax_percent"]=> string(6) "0.0000"
             ["total"]=> string(9) "1033.8500"
             ["date"]=> string(10) "2017-05-11"
             ["category"]=> string(1) "3"
             ["description"]=> string(11) "Credit Card"
             ["period_from"]=> string(10) "0000-00-00"
             ["period_to"]=> string(10) "0000-00-00"
             ["service_id"]=> string(1) "0"
             ["payment_id"]=> string(3) "366"
             ["invoice_id"]=> string(1) "0"
             ["invoiced_by_id"]=> string(1) "0"
             ["comment"]=> string(15) "Pay by Credit Card"
             ["to_invoice"]=> string(1) "0"
             ["service_type"]=> string(8) "internet"
             ["source"]=> string(6) "manual"
             ["balance"]=> NULL
             ["total_with_tax"]=> NULL
             ["ips_to_remove":"db\ActiveTable":private]=> array(0) { }
             ["relatedItems":protected]=> array(0) { }
             ["deleted"]=> string(1) "0"
             ["_relations":"db\Record":private]=> array(0) { }
             ["connected_models":"db\Record":private]=> NULL
             ["_oldAttributes":protected]=> array(22) { [
                     some old attributes ...
                     }
             ["_errors":"base\Model":private]=> NULL     
             ["_additionalAttributes":protected]=> array(0) { }
             ["_isAdditionalAttributesLoaded":protected]=> bool(false)
             }
     [681]=> object(models\common\finance\Transactions)#224 (32) {
             The same attributes
             }
     [985]=> object(models\common\finance\Transactions)#223 (32) {
             The same attributes
             }
</p>


####Invoices variables:
details<br>
summary>{{ dump(loader.invoices) }}</summary<br>
p markdown="1">

##### result will be array of invoices variables fields:

     array(1) { [685]=> object(models\common\finance\Invoices)#226 (29) {
     ["id"]=> string(4) "685"
     ["customer_id"]=> string(1) "4"
     ["date_created"]=> string(10) "2017-05-31"
     ["real_create_datetime"]=> string(19) "2017-06-01 00:00:13"
     ["date_updated"]=> string(10) "2017-06-01"
     ["date_payment"]=> string(10) "2017-05-31"
     ["date_till"]=> string(10) "2017-06-15"
     ["use_transactions"]=> string(1) "1"
     ["note"]=> string(0) ""
     ["memo"]=> string(0) ""
     ["number"]=> string(12) "201713000183"
     ["total"]=> string(8) "533.6000"
     ["payment_id"]=> string(1) "0"
     ["payd_from_deposit"]=> string(1) "1"
     ["status"]=> string(4) "paid"
     ["mark"]=> NULL
     ["recalculated"]=> bool(false)
     ["noCache"]=> bool(false)
     ["is_sent"]=> string(1) "0"
     ["disable_cache"]=> NULL
     ["ips_to_remove":"db\ActiveTable":private]=> array(0) { }
     ["relatedItems":protected]=> array(0) { }
     ["deleted"]=> string(1) "0"
     ["_relations":"db\Record":private]=> array(0) { }
     ["connected_models":"db\Record":private]=> NULL
     ["_oldAttributes":protected]=> array(17) {
             some old attributes ...
             }
     }
</p>
</details>

####Invoice items:
details<br>
summary>{% for invoice in loader.getInvoices() %} ...</summary<br>
p markdown="1">

##### {% for invoice in loader.getInvoices() %}
     Invoice {{ invoice.number}} items:
     {{ dump(invoice.items) }}
     {% endfor %}
     {{ dump(loader.invoices) }}



     result will be array of tariff field and invoices fields:

     Invoice 201713000183 items:
     array(1) {
     [0]=> array(12) {
             ["id"]=> string(4) "948"
             ["invoice_id"]=> string(4) "684"
             ["pos"]=> string(1) "0"
             ["description"]=> string(9) "Internet tariff - 30Mb"
             ["quantity"]=> string(1) "1"
             ["unit"]=> string(0) ""
             ["price"]=> string(8) "464.0000"    
             ["tax"]=> string(7) "15.0000"
             ["period_from"]=> string(10) "2017-05-14"
             ["period_to"]=> string(10) "2017-05-31"
             ["transaction_id"]=> string(4) "984"
             ["deleted"]=> string(1) "0"
             }
     }
     array(1) {
     [948]=> object(models\common\finance\Invoices)#280 (29) {
             ["id"]=> string(4) "948"
             ["customer_id"]=> string(1) "4"
             ["date_created"]=> string(10) "2017-05-31"
             ["real_create_datetime"]=> string(19) "2017-06-01 00:00:13"
             ["date_updated"]=> string(10) "2017-06-01"
             ["date_payment"]=> string(10) "2017-05-31"
             ["date_till"]=> string(10) "2017-06-15"
             ["use_transactions"]=> string(1) "1"
             ["note"]=> string(0) ""
             ["memo"]=> string(0) ""
             ["number"]=> string(12) "201713000183"
             ["total"]=> string(8) "533.6000"
             ["payment_id"]=> string(1) "0"
             ["payd_from_deposit"]=> string(1) "1"
             ["status"]=> string(4) "paid"
             ["mark"]=> NULL
             ["recalculated"]=> bool(false)
             ["noCache"]=> bool(false)
             ["is_sent"]=> string(1) "0"
             ["disable_cache"]=> NULL
             ["ips_to_remove":"db\ActiveTable":private]=> array(0) { }
             ["relatedItems":protected]=> array(0) { }
             ["deleted"]=> string(1) "0"
             ["_relations":"db\Record":private]=> array(0) { }
             ["connected_models":"db\Record":private]=> NULL
             ["_oldAttributes":protected]=> array(17) {
                     some old attributes ...
                     }
             }
     }
</p>
</details>

####Pro-formas:
details<br>
summary>{{ dump(loader.requests) }}</summary<br>
p markdown="1">

##### result will be array of pro-forma fields:

     array(1) {
     [2]=> object(models\common\finance\Requests)#226 (23) {
             ["id"]=> string(1) "2"
             ["customer_id"]=> string(1) "4"
             ["date_created"]=> string(10) "2017-06-07"
             ["real_create_datetime"]=> string(19) "2017-06-07 14:56:25"
             ["date_updated"]=> string(10) "2017-06-07"
             ["date_payment"]=> string(10) "0000-00-00"
             ["date_till"]=> string(10) "2017-06-22"
             ["number"]=> string(10) "2017000002"
             ["total"]=> string(8) "180.0000"    
             ["payment_id"]=> string(1) "0"
             ["status"]=> string(8) "not_paid"
             ["is_sent"]=> string(1) "0"
             ["note"]=> string(4) "Note"
             ["memo"]=> string(4) "Memo"
             ["ips_to_remove":"db\ActiveTable":private]=> array(0) { }
             ["relatedItems":protected]=> array(0) { }
             ["deleted"]=> string(1) "0"
             ["_relations":"db\Record":private]=> array(0) { }   
             ["connected_models":"db\Record":private]=> NULL
             ["_oldAttributes":protected]=> array(15) {
                     some old attributes ...
                     }
             ["_errors":"base\Model":private]=> NULL
             ["_additionalAttributes":protected]=> array(0) { }
             ["_isAdditionalAttributesLoaded":protected]=> bool(false)
             }
     }
</p>
</details>

####Payments:
details<br>
summary>{{ dump(loader.payments) }}</summary<br>
p markdown="1">

##### result will be array of payment fields:

     array(1) {
     [366]=> object(models\common\finance\Payments)#226 (28) {
             ["id"]=> string(3) "366"
             ["customer_id"]=> string(1) "4"
             ["invoice_id"]=> string(1) "0"
             ["request_id"]=> string(1) "0"
             ["transaction_id"]=> string(4) "2400"
             ["payment_type"]=> string(2) "10"
             ["receipt_number"]=> string(13) "2017-10-00011"
             ["date"]=> string(10) "2017-05-13"
             ["real_create_datetime"]=> string(19) "2017-05-13 09:19:02"
             ["amount"]=> string(9) "1033.8500"
             ["comment"]=> string(15) "Pay by Bank Transfer"
             ["is_sent"]=> string(1) "1"
             ["field_1"]=> string(0) ""
             ["field_2"]=> string(10) "UNIC00032"
             ["field_3"]=> string(10) "UNIC00032"
             ["field_4"]=> string(13) "Payment: null"
             ["field_5"]=> string(19) "Bank Statement: 23"
             ["note"]=> string(0) ""
             ["memo"]=> string(0) ""
             ["ips_to_remove":"db\ActiveTable":private]=> array(0) { }
             ["relatedItems":protected]=> array(0) { }
             ["deleted"]=> string(1) "0"
             ["_relations":"db\Record":private]=> array(0) { }
             ["connected_models":"db\Record":private]=> NULL
             ["_oldAttributes":protected]=> array(20) {
                     some old attributes ...
                     }
             ["_errors":"base\Model":private]=> NULL
             ["_additionalAttributes":protected]=> array(0) { }
             ["_isAdditionalAttributesLoaded":protected]=> bool(false)
             }
     }
</p>
</details>

####Attached documents:
details<br>
summary>Invoices: {{ dump(loader.getAttac ...</summary<br>
p markdown="1">

##### Invoices:
     {{ dump(loader.getAttachedInvoices) }}
     Pro-formas:
     {{ dump(loader.getAttachedRequests) }}
     Payment receipts:
     {{ dump(loader.getAttachedReceipts) }}




     result will be array of attached documents fields:

     array(1) {

     }
</p>
</details>


####Ignore Notification
details<br>
summary>Ignore Notification</summary<br>
p markdown="1">

##### Example:
     {% if customer.billing_type == 'prepaid' %}
     === IGNORE NOTIFICATION ===
     {% else %}
     example  {{ customer.login }}
     {% endif %}



if the template result is "=== IGNORE NOTIFICATION ===" the notification will not be sent

</p>
</details>



And now, you can see **examples** how to use variables in templates:
```
Hello!

This is example template. We use Twig as template engine!
You can use some variables in templates.
For example to get customer name use {{ customer.name }},
customer login - {{ customer.login }}.
```

```
{% set billing_custom = loader.billing %}

Hello {{ customer.name}},
your deposit is {{ billing_custom.deposit }} EUR,
we strongly recommended to refill it.
```

```

{{ App.t('common', 'Hello') }} {{ customer.name }},
We would like to welcome you as a Super ISP!
Your Billing date will be {{ loader.billing.billing_date }} of every month.
There is no fixed length contract and you will be billed 1 month in advance.
Your customer reference number is {{ loader.customer.id }}
The e-mail address to where your invoices will be sent is : {{ loader.customer.email }}
Your Wifi password is: {{ loader.customer.additionalAttributes.wifi_pass }}


To download your invoices, view payments, create support tickets, see your usage statistics, use our customer self service portal my.splynx.com using username {{ loader.customer.login }} and {{ loader.customer.password }} as your password.

Our phone numbers in case you have not saved them yet,

1234567890
1234567890

office@superisp.com
```



####Here you can find example of Document - Contract:
details<br>
summary>Template of a Contract</summary<br>
<div markdown="1">

```bash     
     <!DOCTYPE html>
     <html lang="en">
     <head>
     <meta charset="UTF-8">
     <title></title>
     <style>
     td, th, tr {
     border: 1px solid black;
     word-wrap: break-word;
     }

     table {
     border-collapse: collapse;
     table-layout: fixed;
     font-family: Arial, Verdana, sans-serif;
     font-size: 10px;
     }

     .fs {
     font-family: Arial, Verdana, sans-serif;
     font-size: 10px;
     }

     body {
     margin: 10px;
     padding: 10px;
     }
     </style>
     </head>
     <body>
     <div style="text-align: center" class="fs"><h4>SUBSCRIBER CONTRACT AGREEMENT No. {{ customer.id }} </h4>
     entered into between
     </div>
     <br>
     <div>
     <table style="width:100%">
     <tr>
     <td bgcolor="#e0e0e0" style="width: 15%"><b>Company Name:</b></td>
     <td colspan="3">BEST ISP</td>
     </tr>
     <tr>
     <td bgcolor="#e0e0e0"><b>VAT id:</b></td>
     <td colspan="3">123455667</td>
     </tr>
     <tr>
     <td bgcolor="#e0e0e0"><b>Address</b></td>
     <td colspan="3">5 Main Street, Gotham city, 12345</td>
     </tr>
     <tr>
     <td bgcolor="#e0e0e0"><b>Phone number:</b></td>
     <td colspan="3">123456788</td>
     </tr>
     <tr>
     <td bgcolor="#e0e0e0"><b>Email</b></td>
     <td colspan="3">office@bestisp.com</td>
     </tr>
     <tr>
     <td bgcolor="#e0e0e0"><b>Date</b></td>
     <td style="width: 30%">{{ "now"|date("m/d/Y") }}</td>
     <td bgcolor="#e0e0e0" style="width: 10%"><b>Place</b></td>
     <td>Gotham city</td>
     </tr>
     <tr>
     <td bgcolor="#e0e0e0"><b>Signature</b><br>Employee of BEST ISP</td>
     <td colspan="3"></td>
     </tr>
     </table>
     </div>
     <br>
     <div style="text-align: center">(<b>"SERVICE PROVIDER"</b>) and
     </div>
     <br>
     <div>
     <table style="width:100%">
     <tr>
     <td bgcolor="#e0e0e0" style="width: 15%"><b>Name and Surname /<br>Company name</b></td>
     <td colspan="3">{{ customer.name }}</td>
     </tr>
     <tr>
     <td bgcolor="#e0e0e0"><b>Connection Address</b></td>
     <td colspan="3"> {{ loader.customer.street_1 }}{% if loader.customer.additionalAttributes.street_2 is not empty %}, {{ loader.customer.additionalAttributes.street_2 }}{% endif %}, {{ customer.city}}{% if loader.customer.zip_code is not empty %}, {{ loader.customer.zip_code }}{% endif %}</td>
     </tr>

     <tr>
     <td bgcolor="#e0e0e0"><b>Email</b><br>Invoices and receipts will be sent to this address</td>
     <td colspan="3">{{ loader.customer.email }}</td>
     </tr>
     <tr>
     <td bgcolor="#e0e0e0"><b>Phone</b></td>
     <td colspan="3">{{ loader.customer.phone }}</td>
     </tr>
     {% if loader.customer.additionalAttributes.contact_2 is not empty %}
     <tr>
     <td bgcolor="#e0e0e0"><b>Authorized person:</b></td>
     <td colspan="3">{{ loader.customer.additionalAttributes.contact_2 }}</td>
     </tr>
     {% endif %}
     {% if loader.customer.additionalAttributes.phone_2 is not empty %}
     <tr>
     <td bgcolor="#e0e0e0"><b>Authorized person's phone</b></td>
     <td colspan="3">{{ loader.customer.additionalAttributes.phone_2 }}</td>
     </tr>
     {% endif %}
     {% if loader.customer.additionalAttributes.contact_3 is not empty %}
     <tr>
     <td bgcolor="#e0e0e0"><b>Second Authorized person:</b></td>
     <td colspan="3">{{ loader.customer.additionalAttributes.contact_3 }}</td>
     </tr>
     {% endif %}
     {% if loader.customer.additionalAttributes.phone_3 is not empty %}
     <tr>
     <td bgcolor="#e0e0e0"><b>Second uthorized person's phone:</b></td>
     <td colspan="3">{{ loader.customer.additionalAttributes.phone_3 }}</td>
     </tr>
     {% endif %}
     <tr>
     <td bgcolor="#e0e0e0"><b>Date</b></td>
     <td style="width: 30%">{{ "now"|date("m/d/Y") }}</td>
     <td bgcolor="#e0e0e0" style="width: 10%"><b>Place</b></td>
     <td>Gorey</td>
     </tr>
     <tr>
     <td bgcolor="#e0e0e0"><b>WiFi Password</b></td>
     <td colspan="3">{{ loader.customer.additionalAttributes.wifi_pass }}</td>
     </tr>
     <tr>
     <td bgcolor="#e0e0e0"><b>Login to my BEST ISP</b></td>
     <td style="width: 30%">{{loader.customer.login}}</td>
     <td bgcolor="#e0e0e0" style="width: 10%"><b>Password to my BEST ISP</b></td>
     <td> {{loader.customer.password}}</td>
     </tr>
     <tr>
     <td bgcolor="#e0e0e0"><b>Signature</b><br>Who warrants he/she is duly authorized hereto</td>
     <td colspan="3"></td>
     </tr>
     </table>
     </div>
     <br>
     <div style="text-align: center" class="fs">(<b>"SUBSCRIBER"</b>)<br>
     (together the <b>"Parties"</b>. A reference to <b>"Party"</b> shall be a reference to one of them as so determined
     by the context.)<br>For the period and services selected below
     </div>



     <div class="fs">
     <h4><b><br>
     {% set active_services = loader.getServicesByTypeAndStatus('internet', 'active') %}
     {% for active in active_services %}
     Service: {{ active.type }}<br>
     Tarriff: {{ active.description }}<br>
     Monthly price: {{ active.unit_price }}<br>
     Service start date: {{ active.start_date }}<br>
     {% endfor %}
     {% set active_voice = loader.getServicesByTypeAndStatus('voice', 'active') %}
     {% for voice in active_voice %}
     {% if voice is not empty %}
     Service: {{ voice.type }}<br>
     Tarriff: {{ voice.description }}<br>
     Monthly price: {{ voice.unit_price }}<br>
     Service start date: {{ voice.start_date }}<br>
     {% endif %}
     {% endfor %}
     Contract Term: {{ loader.customer.additionalAttributes.contract_term }}
     </h4></b>
     </div>
     <div style="position: fixed; bottom: 0; width: 100%;" class="fs">
     <div style="text-align: right"></div>
     <hr style="width: 100%"/>
     <div>BEST ISP BROADBAND SERVICE AGREEMENT</div>
     <div style="text-align: right">Page 1 of 8</div>
     </div>
     <div style="page-break-before: always;"></div>

     <div style="text-align: justify"><h4>TERMS AND CONDITIONS FOR ???????BEST FIBRE???????? SERVICES</h4>
     This Subscriber Agreement (???????Agreement???????) is made by and between Subscriber and JS BEST ISP Limited. (???????BEST ISP???????), for?? the provision and use of ???????BRDY Fibre???????? Internet access (the ???????Service???????).
     Now therefore, in consideration of the?? mutual promises and covenants herein contained, the adequacy of which is hereby acknowledged, and intending?? to be legally bound, Subscriber and BEST ISP hereby agree as follows:
     <h4>1. AGREEMENT.</h4>Subscriber agrees to be bound by this Agreement and to use the Service in compliance with the terms of this?? Agreement and with BEST ISP????????s Acceptable Usage Policy and any modifications made to same from time to time.
     <h4>2. THE SUBSCRIBER.</h4>The Subscriber is at least 18 years of age, is legally able to enter into contracts and is responsible for this Subscriber?? account. The Subscriber shall pay all fees, taxes, charges and other expenses incurred in connection with the?? account.
     <h4>3. SUBSCRIBER ACKNOWLEDGEMENTS REGARDING THE SERVICE.</h4>
     (a)?? The Service consists of a VDSL internet connection over a copper phone line. While BEST ISP will undertake all?? reasonable commercial efforts to deliver the stated service the Subscriber acknowledges that service speed can?? vary depending on distance, Internet traffic and other factors beyond the control of BEST ISP. The Service may?? contain material that is unsuitable for minors and The Subscriber acknowledges that BEST ISP does not and cannot?? filter the content.
     <br>
     (b)?? The Subscriber acknowledges that in order to provide the Service, BEST ISP has contracted with communications?? and network operators for internet access. The Subscriber further acknowledges that BEST ISP will only provide?? uninterruptible continuous Service to The Subscriber pursuant to this Agreement to the extent which BEST ISP receives?? such service from linked communications and network operators.
     <br>
     (c) The ?? Subscriber acknowledges and agrees that from time to time BEST ISP may be required to temporarily suspend?? the Service to subscriber to verify compliance with applicable licenses, authorizations, and compliance with the?? technical and operating parameters of the network. Under such circumstances BEST ISP will use all reasonable?? efforts to minimize disruption to the Service including making reasonable efforts that any such suspension take?? place out of normal business hours.
     <br>
     (d)?? The Subscriber accepts that BEST ISP may change or withdraw any element of the Service from time to time and?? will use all reasonable efforts to notify Subscriber of any necessary change in the Services.
     <br>
     (e) The Subscriber?? acknowledges that the Service is an ???????always open??????? connection to the internet while the equipment is powered on?? and that it is Subscriber????????s SOLE RESPONSIBILITY to install, configure and maintain suitable security measures?? to protect The Subscriber????????s computer and equipment from unauthorised or malicious access from the internet. Any?? advice or equipment provided by BEST ISP is provided ???????as is???????? and BEST ISP accepts no responsibility or liability for?? the security of Subscriber????????s systems.

     <div style="position: fixed; bottom: 0; width: 100%;" class="fs">
     <div style="text-align: right"></div>
     <hr style="width: 100%"/>
     <div>BEST ISP BROADBAND SERVICE AGREEMENT</div>
     <div style="text-align: right">Page 2 of 8</div>
     </div>
     <div style="page-break-before: always;"></div>
     <h4>4. EQUIPMENT.</h4>
     (a)?? From service activation BEST ISP will loan certain VDSL modem and associated equipment, hereafter termed?? ???????Equipment???????, to The Subscriber to access the service. This Equipment at all times remains the sole property of?? BEST ISP and The Subscriber agrees to provide BEST ISP access and permission to recover said equipment on demand?? without delay, obstruction or interference.
     <br>
     (b) The ?? Subscriber agrees to use the Equipment in accordance with BEST ISP????????s instructions and to restrict access to?? the Equipment to only those representatives and agents authorized by BEST ISP. The Subscriber agrees to take?? reasonable steps to protect the Equipment from damage, loss or theft.
     <br>
     (c)?? The Subscriber agrees to notify BEST ISP as soon as reasonably possible once he becomes aware of any damage?? to the equipment or defect in the operation of the equipment by telephoning or emailing BEST ISP at the numbers?? or addresses published from time to time, or office@bestisp.com
     <br>
     (d)?? On termination or cancellation of the Service Contract for any reason whatsoever, it is the responsibility of the?? Subscriber to return by recorded mail in good condition and suitably packaged, the VDSL Modem and any other?? related equipment provided by BEST ISP. Failure to return equipment within 14 days of the service?? termination/cancellation date will generate an automatic equipment fee of ???????99 including VAT which will be?? deducted from The Subscribers account and The Subscriber hereby agrees to same.
     <br>
     <h4>5. TERM.</h4>
     (a)?? This Agreement is for an initial term of 6, 12 or 18 months, as defined by your price plan rules, and shall?? automatically renew for subsequent month term, until terminated in accordance with this Agreement. After the?? Initial Term, The Subscriber may terminate this Agreement upon thirty (30) days written notice to BEST ISP.
     <br>
     (b)?? Should The Subscriber terminate this agreement for any reason during the initial term, a cancellation fee equal to?? the remainder of the contract term will become immediately due, and The Subscriber acknowledges and agrees to?? pay such fee and return any equipment provided.
     <br>
     (c)?? The Subscriber may upgrade the service at any time to a higher service and accepts that a new contract applies?? from the date the upgrade is applied.
     <br>
     (d)?? BEST ISP may in its sole discretion terminate this Agreement at any time. In the event that BEST ISP terminates?? this Agreement for reasons other than breach of this Agreement by Subscriber, then BEST ISP shall endeavour to?? the extent reasonably possible to provide 30 days notice to The Subscriber. The Subscriber is liable under this Agreement?? for all fees and charges until such time as the Agreement has been terminated. THE SUBSCRIBER UNDERSTANDS THAT UNLESS WRITTEN NOTIFICATION IS RECEIVED BY BEST ISP AFTER THE INITIAL TERM, THE?? SERVICE SHALL CONTINUE AND SUBSCRIBER WILL CONTINUE TO BE RESPONSIBLE FOR PAYMENT?? OF APPLICABLE SERVICE FEES.
     <br>
     <div style="position: fixed; bottom: 0; width: 100%;" class="fs">
     <div style="text-align: right"></div>
     <hr style="width: 100%"/>
     <div>BEST ISP BROADBAND SERVICE AGREEMENT</div>
     <div style="text-align: right">Page 3 of 8</div>
     </div>
     <div style="page-break-before: always;"></div>
     <h4>6. TERMINATION.</h4><br>
     (a)?? If Subscriber is dissatisfied with the Service or any related terms, conditions, rules, policies, guidelines, or?? practices, and if these issues cannot be resolved through BEST ISP????????s Customer Complaints procedure,?? The Subscriber????????s sole remedy is to discontinue using the Service, cancel the account, and pay any cancellation fees?? that apply. To cancel the Service The Subscriber must send a written request for termination by email to BEST ISP?? and same must be signed by an authorised representative of The Subscriber to arrive not less than 5 working days?? before the end of the current billing term. Should The Subscriber terminate this agreement during the initial term for?? any reason other than a failure by BEST ISP to provide Internet Access service for a period in excess of 5 days, a?? cancellation fee equal the remainder of the contract term will become immediately due, and The Subscriber?? acknowledges and agrees to pay such fee.
     <br>
     (b)?? Upon cancellation or otherwise upon termination of this Agreement, related email and hosting services will be?? terminated and all the Subscriber files stored on BEST ISP servers may be deleted. BEST ISP may terminate this?? Agreement, your password, your account, or your use of the Services for any reason, including, without limitation,?? if BEST ISP, in its sole discretion, believes you have violated the Agreements or if The Subscriber fails to pay any?? charges when due.
     <br>
     (c)?? Sections 11, 20, 21, and 22 of this Agreement shall survive termination of this Agreement.
     <br>
     (d)?? BEST ISP may terminate this agreement immediately if The Subscriber is subject to bankruptcy, insolvency,?? examinership, receivership, liquidation or any similar proceedings, or in BEST ISP????????s exclusive opinion is unable to?? pay fees due to BEST ISP.
     <br>
     <h4>7. FEES AND PAYMENT</h4><br>
     (a)?? Subscriber shall pay a monthly service fee and all other applicable fees, charges, taxes, and other amounts?? for the Service at the rates in effect for the current billing period. BEST ISP may increase or decrease the monthly?? service fee. BEST ISP will use all reasonable efforts to provide The Subscriber thirty (30) days or more notice of same.?? If such changes to the basic monthly service fee are to The Subscribers detriment (e.g. a price increase), The Subscriber?? may terminate this agreement by giving thirty (30) days written notice, and The Subscriber will remain liable only for?? any balance on the account.
     <br>
     (b)?? Payment is due in full by Credit Card or Direct Debit at the start of each billing month. All charges are?? considered valid unless disputed in writing within thirty (30) days of the billing date. Adjustments will not be made?? for charges that are more than 30 days old. If any payment is more than 7 days overdue or is returned by the?? bank unpaid, the Service may be suspended with immediate effect and remain suspended until the due amounts?? are paid in full. The Subscriber is not relieved of the obligation to pay the monthly service fee while an account is?? suspended. BEST ISP may at its sole discretion terminate the Service and this Agreement for any accounts which?? are 14 days or more overdue. A reactivation fee or deposit may be required before Service is reactivated after?? suspension or termination. Credit account balances shall not accrue interest. The Subscriber agrees to pay the?? reasonable costs of any collection agency, solicitor or court used by BEST ISP to collect past due amounts or to?? enforce this Agreement. Returned cheques or Direct Debits will incur a ???????5 administration fee.
     <br>
     (c)?? A ???????1.50 inclusive of VAT charge applies to all bills for non-Direct Debit customers.(d)?? Where a package is downgraded within contract, a ???????30 inclusive of VAT downgrade fee applies.
     <br>
     <div style="position: fixed; bottom: 0; width: 100%;" class="fs">
     <div style="text-align: right"></div>
     <hr style="width: 100%"/>
     <div>BEST ISP BROADBAND SERVICE AGREEMENT</div>
     <div style="text-align: right">Page 4 of 8</div>
     </div>
     <div style="page-break-before: always;"></div>
     <h4>8. SUBSCRIBER ACCOUNT.</h4><br>
     <br>(a)?? The Subscriber will receive a username, password, account reference, and various other account details.?? The Subscriber is solely responsible for use of the Service and for ensuring their information is kept confidential.?? The Subscriber must notify BEST ISP immediately upon discovering any unauthorized use of their account.
     <br>(b) The ?? Subscriber acknowledges that usernames, passwords and IP addresses may change or be changed from?? time to time, and specifically that fixed IP addresses are not guaranteed except in the case of custom services?? where this specifically comprises part of the service contract.
     <br>
     <h4>9. FAIR ACCESS POLICY.</h4><br>
     To ensure equal Internet access for all subscribers, BEST ISP operates a fair access policy. Fair access?? establishes an equitable balance in Internet access across high speed Internet services for all subscribers. To?? ensure this equity, certain types of traffic such as email and browsing may be prioritized over other traffic.?? BEST ISP provides the Service on a ???????best effort??????? basis and does not guarantee upload or download speeds.??
     <br>
     <h4>10. CUSTOMER COMPLAINT POLICY.</h4><br>
     Should you be dissatisfied for any reason with the service provided by BEST ISP, a formal complaint process is?? provided to ensure that your issue is addressed as quickly as possible and at the highest level necessary. This is?? outlined as follows:
     <br>
     (a)?? GENERAL: If you have a general complaint regarding BEST ISP, email full details and your account reference?? us at office@bestisp.com. Issues registered in this way automatically enter BEST ISP????????s complaint tracking?? systems, ensuring the most appropriate and quickest handling.
     <br>
     (b)?? BILLING: If you have a billing enquiry or complaint, please contact the Accounts Department via the number?? shown on your invoice/statement, or by email to office@bestisp.com.
     <br>
     (c)?? WRITTEN: If you would prefer to put your complaint in writing, we will respond to your letter by telephone and?? will confirm any details in writing should you wish. Your letter should be addressed to: Best ISP, Main street Gotham city
     <br>
     (d)?? IDENTITY: If telephoning BEST ISP, each staff contact receiving your call will provide his or her name on?? request. Record same for future reference or to revert later to the same person working on your query or?? complaint.
     <br>
     (e)?? RESOLUTION: The staff member receiving your call will either resolve your complaint or transfer your?? complaint to a more appropriate person to endeavour to resolve your complaint to your satisfaction. Where?? possible, our staff will resolve your concern at the first point of contact.
     <br>
     (f)?? ESCALATION: If you are not satisfied with the resolution, or if you feel that you have not received a fair?? hearing, your complaint can be escalated to a manager on your request. He or she will review your?? complaint and resolutions offered and discuss the complaint with you.
     <br>
     <div style="position: fixed; bottom: 0; width: 100%;" class="fs">
     <div style="text-align: right"></div>
     <hr style="width: 100%"/>
     <div>BEST ISP BROADBAND SERVICE AGREEMENT</div>
     <div style="text-align: right">Page 5 of 8</div>
     </div>
     <div style="page-break-before: always;"></div>
     <h4>11. INSTALLATION.</h4>
     (a)?? The installation, use, inspection, maintenance, repair, and removal of the equipment may result in service?? outage or potential damage to your computer. The Subscriber is solely responsible for backing up all existing?? computer files and data. BEST ISP and its employees, agents, contractors, and representatives shall have no?? liability whatsoever for any damage to or loss or destruction of any of your hardware, software, files, data, or?? peripherals.
     <br>
     (b)?? BEST ISP will endeavour to provide the Service to all eligible applicants, subject to technical and commercial?? feasibility. BEST ISP may in its sole discretion determine that it cannot or will not service a particular site or?? subscriber, and reserves the right to cancel the installation process and refund any money that The Subscriber has?? paid. BEST ISP will notify you of its intent to cancel as soon as reasonably possible. It may take up to 90 or more?? days to determine if BEST ISP is able to provide service in certain locations. BEST ISP shall have no responsibility?? whatsoever for claims arising out of its failure or refusal to complete the installation or provide the Service.
     <h4>12. COPYRIGHTS AND LICENSES.</h4>
     The content on the Service is protected under applicable copyright law. Any copying, modification, distribution,?? publication or other use by The Subscriber, or by any user of The Subscriber????????s account, of any such content is prohibited,?? except as expressly permitted by the holder of the applicable copyrights.
     <h4>13. NO ENDORSEMENT.</h4><br>
     BEST ISP does not endorse or in any way vouch for the accuracy or completeness of any content made available?? through the Service. BEST ISP does not recommend that such content be relied on by The Subscriber without?? appropriate verification.
     <h4>14. SUBSCRIBER CONDUCT.</h4>
     The Subscriber shall comply with all laws, rules, regulations and legal obligations related to the Service and with all?? acceptable use policies and procedures established from time to time by BEST ISP. The Subscriber shall not use the?? Service to conduct any business or activity or to solicit the performance of any activity which is prohibited by any?? law, rule, regulation or legal obligation. The Subscriber shall not intercept email in an unauthorized manner or engage?? in ???????spamming??????? or any similar conduct.
     <h4>15. THIRD PARTY ACCESS</h4>
     (a)The?? Subscriber shall not resell, share, lease, hire or otherwise permit access to the Service to any third party,?? including but not limited to the connection of any third party to the Service through use of direct cable connection,?? network connection, wireless networking, or any other means.
     <br>
     (b)?? BEST ISP reserve the right to suspend the Service pending investigation where it reasonably suspects the?? above clause is breached by The Subscriber and reserves the right to terminate with immediate effect the Service and?? this Agreement where such breach has taken place.
     <div style="position: fixed; bottom: 0; width: 100%;" class="fs">
     <div style="text-align: right"></div>
     <hr style="width: 100%"/>
     <div>BEST ISP BROADBAND SERVICE AGREEMENT</div>
     <div style="text-align: right">Page 6 of 8</div>
     </div>
     <div style="page-break-before: always;"></div>
     <h4>16. SERVICE MONITORING.</h4><br>
     BEST ISP has no obligation to monitor the Service, but may do so and disclose information regarding use of the?? Services for any reason if BEST ISP, in its sole discretion, believes that it is reasonable to do so, including to:?? satisfy laws, regulations, or governmental or legal requests; operate the Service properly; or protect itself and its?? subscribers. BEST ISP may immediately remove your material or information from BEST ISP servers, in whole or in?? part, which BEST ISP, in its sole and absolute discretion, determines to infringe another????????s property rights or to?? violate BEST ISP????????s Acceptable Use Policy.
     <br>
     <h4>17. SUBSCRIBER EQUIPMENT.</h4><br>
     The Subscriber shall maintain and operate suitable and fully compatible terminal equipment and communication?? devices required to access the service. BEST ISP makes no representation or warranties, either express or implied,?? regarding such Subscriber equipment.
     <br>
     <h4>18. DISCLAIMER OF WARRANTIES.</h4><br>
     Access to the service is not guaranteed. The Service is distributed on an ???????as is??????? and ???????as available??????? basis without warranties of any kind, either express or implied, including but not limited to warranties of title or implied?? warranties of merchantability or fitness for a particular purpose or otherwise.
     <br>
     <h4>19. LIMITATION OF LIABILITY.</h4><br>
     Neither BEST ISP nor any of its information or content providers, service providers, licensors, employees or agents?? shall be liable for any direct, indirect, incidental, special, punitive or consequential damages arising out of The?? Subscriber????????s use of the service or inability to use the service or any breach of any representation or warranty. In?? any event, no such liability shall exceed the total amount actually paid by The Subscriber for services provided under?? this agreement for the prior six month period.
     <br>
     <h4>20. INDEMNITY.</h4><br>
     The Subscriber assumes all risk and liability for any use of the Service. The Subscriber agrees to indemnify BEST ISP?? against all claims, liability, damages, costs and expenses, including but not limited to reasonable legal fees,?? arising out of or related to Subscriber????????s use of the Service.
     <br>
     <div style="position: fixed; bottom: 0; width: 100%;" class="fs">
     <div style="text-align: right"></div>
     <hr style="width: 100%"/>
     <div>BEST ISP BROADBAND SERVICE AGREEMENT</div>
     <div style="text-align: right">Page 7 of 8</div>
     </div>
     <div style="page-break-before: always;"></div>
     <h4>21. THIRD PARTY BENEFICIARIES.</h4>
     The provisions of Sections 18, 19 and 20 are for the benefit of BEST ISP and its respective contractors, information?? or content providers, service providers, licensors, employees and agents; and each shall have the right to assert?? and enforce such provisions directly on its own behalf.
     <h4>22. SUPPORT SERVICES.</h4>
     The Subscriber shall direct all enquiries and service related issues to BEST ISP????????s Customer Sales and Support contact points, as defined on its website from time to time or directly by email to office@bestisp.com.
     <h4>23. APPLICABLE LAWS.</h4>
     This Agreement shall be governed by the laws of the Republic of Ireland. Any cause of action of The Subscriber, or by?? users of The Subscriber????????s account, with respect to the Service or this Agreement must be instituted within six (6)?? months after the claim or cause of action has arisen or be barred. It is acknowledged that this is a services contract and not a contract for the sale of goods.
     <h4>24. GENERAL.</h4>
     (a)This Agreement constitutes the entire agreement between the parties relating to the subject matter hereunder,?? and supersedes any and all oral and/or written statements, discussions, representations and agreements made?? by either party to the other, and may not be assigned without the express written consent of BEST ISP. No?? modification of this Agreement shall be binding on either party unless it is in writing and signed by both parties.?? Failure on the part of BEST ISP to enforce any provision of this Agreement shall not be construed as a general?? waiver or relinquishment of the right to enforce such provision. If any provision shall be held unenforceable, the?? validity legality and enforceability of the remaining provisions shall in no way be affected thereby, and the intent?? of the unenforceable provision enacted to the maximum enforceable extent.
     <br>
     (b)?? Publicity. BEST ISP may identify The Subscriber as a user of BEST ISP????????s services in reports, advertisements and other?? promotional literature or forms of publication. The Subscriber should advise BEST ISP in writing if it does not wish to be?? identified.
     <br>
     (c)?? These Terms and Conditions may be modified by BEST ISP from time to time, the current and applicable?? version always being available in electronic form from the relevant section of the BEST ISP website at?? www.wi.ie. BEST ISP will make reasonable attempts by email or other communication, including but not?? limited to national press, to inform The Subscriber when the Terms and Conditions of the Service are amended.?? Should any modification cause a reasonable deterioration in the level of the Service the Subscriber could?? reasonably expect, their sole remedy is to terminate service in writing within 30 days of such change. Should?? The Subscriber continue to use the Service 30 days following date of notice of an amendment made to the Terms and?? Conditions the Subscriber is deemed to have accepted the amended terms.
     <br>
     (d)?? Headings for Convenience. All headings preceding paragraphs and subparagraphs have been inserted for?? convenience of reference only, and shall not be relied upon in determining the meaning of the rights and?? obligations of BEST ISP or Subscriber.
     </div>
     <div style="position: fixed; bottom: 0; width: 100%;" class="fs">
     <div style="text-align: right"></div>
     <hr style="width: 100%"/>
     <div>BEST ISP BROADBAND SERVICE AGREEMENT</div>
     <div style="text-align: right">Page 8 of 8</div>
     </div>
     </body>
     </html>
     ```
