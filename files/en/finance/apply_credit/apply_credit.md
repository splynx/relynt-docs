Applying Credit
=============

## How to apply Credit to future invoices

In relation to the account balances of customers, in certain cases you may have a customer with a positive balance, however, it is not enough to pay for the cost of their services on the next invoice. The logical solution would be to deduct this positive balance to be from the total of the next invoice.

Here is an illustration the process of applying credit to a customer's account.


For example, the customer's account balance is $10:


![Preview](1.png)

From the list of transactions you can see That the customer's payment was more than invoiced amount:

![Preview](2.png)

From the Services tab, you can see the service price is 100:

![Preview](3.png)

If you were to charge the customer for the next invoice, you will see the price of the service again on the invoice preview:

![Preview](4.png)


To resolve this issue and apply the 10€ as credit to the future invoice,  we should follow the steps below:

1. Create a Debit transaction with the same Total as account balance (Description and Category doesn't really matter, this is for your personal reference):

![Preview](5.png)

This will remove the credit from the account balance of the customer.

![Preview](51.png)

2. Create a Credit transaction with the same Total as the credit that was available/= to the debit transaction, but it is absolutely **critical to enable the "Add To invoice" toggle**:

![Preview](6.png)

That's all you need to do  - only two transactions. Then we can check the customer's balance (it will be back to what it was before creating the debit transaction - 10€):

![Preview](7.png)

The final step will be to charge the customer for the future invoice with the "Charge & Invoice" button in the Billing overview tab or simply wait for the next billing day for the system to create the invoice automatically:

![Preview](8.png)

As you can see - the new invoice includes the Credit correction transaction and the reduced total amount.

_Notice: Please don't worry if the preview via the Charge & invoice button does not show the Credit transaction - it is normal. The invoice will be correct with Credit transaction, if these steps were taken._

## How to apply credit to customer accounts with invoices

Credit notes can be created in Relynt by means of invoices.

When you create a invoice in Relynt with a negative amount (-), Relynt automatically changes the tax invoice to a credit note.

To apply credit with invoices, please follow the steps below:

1. Navigate to the respective customer's billing tab and enter the invoice section.

2. Add a one time invoice by clicking on the  "Add one-time invoice" button located about the table on the right, a window will appear for you to add the details:

![Add credit](9.png)

![Add credit](10.png)

Dates can be specified if need be. Notes for the customer and a memo for yourself is recommended. Add a description of your choice for the credit note. The period is optional and the most important part is to add a amount with a negative value "-".

Once the invoice has been created it will appear in the list of invoices and can be operated with the tools in the actions column.

![Add credit](11.png)

The customer will now have an updated account balance with the amount added to the total.

![Add credit](12.png)
