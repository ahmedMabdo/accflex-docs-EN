# Post-Dated Cheques Wallet

**Screen usage:** It is used to manage and track checks received from customers, but their due date has not yet arrived, meaning they are post-dated checks. The primary purpose of this screen is to organize the movement of these checks and track them from the moment they are received until the date they are deposited in the bank, ensuring the accuracy of accounting linkage and financial follow-up.\
**Screen location:** Cash Management → Bank Transactions → Bank Checks → Postdated Checks Wallet

<figure><img src="../../../../.gitbook/assets/image (502).png" alt=""><figcaption></figcaption></figure>

**How to use:**\
&#xNAN;_&#x4D;ain data_: Both the wallet number, date, and bank are all mandatory fields. The bank is selected from the dropdown list within the bank field, which references the banks previously defined under **Cash Management → System Settings → Basic Data → Bank**.

The number of checks and any additional notes can be entered if needed.\
The total deposited amount is calculated and displayed automatically based on the due dates of the checks included in the wallet.

Detailed data:

<table data-header-hidden><thead><tr><th valign="top"></th><th valign="top"></th><th valign="top"></th><th valign="top"></th><th valign="top"></th></tr></thead><tbody><tr><td valign="top">Receivable Note Number</td><td valign="top">Drop-down list</td><td valign="top">Mandatory</td><td valign="top">A financial document issued upon receiving a payment from a customer, whether in cash, by check, or by any other method.<br>Its purpose is to document the receipt of funds and record it in the accounting system.</td><td valign="top"><p>The receipt voucher is issued from: Cash Management → Banking Transactions → Bank Checks → Receivable note.</p><p> </p></td></tr><tr><td valign="top">Check Number</td><td valign="top">Automatic</td><td valign="top">Automatic</td><td valign="top">This is the unique number printed on the check by the bank.</td><td valign="top">The data in this field appears automatically based on what was recorded in the Receivable Note screen.</td></tr><tr><td valign="top">Customer Name</td><td valign="top">Automatic</td><td valign="top">Automatic</td><td valign="top">Represents the name of the person or entity that issued the check.</td><td valign="top">The data in this field appears automatically based on what was recorded in the Receivable Note screen.</td></tr><tr><td valign="top">Currency</td><td valign="top">Automatic</td><td valign="top">Automatic</td><td valign="top">Indicates the currency in which the check was written.</td><td valign="top">The data in this field appears automatically based on what was recorded in the Receivable Note screen.</td></tr><tr><td valign="top">Total Amount</td><td valign="top">Automatic</td><td valign="top">Automatic</td><td valign="top">This is the check amount — the total value to be received upon collection.</td><td valign="top">The data in this field appears automatically based on what was recorded in the Receivable Note screen.</td></tr><tr><td valign="top">Due Date</td><td valign="top">Automatic</td><td valign="top">Automatic</td><td valign="top">Indicates the date specified on the check when the amount can be collected from the bank.</td><td valign="top">The data in this field appears automatically based on what was recorded in the Receivable Note screen.</td></tr><tr><td valign="top">Deposited</td><td valign="top">Automatic</td><td valign="top">Automatic</td><td valign="top"> </td><td valign="top">This check box is automatically maeked once the due date of the check has been reached.</td></tr><tr><td valign="top">Delete Button</td><td valign="top">Press Button</td><td valign="top">Optional</td><td valign="top"> </td><td valign="top">Used when the user wishes to delete the selected row.</td></tr></tbody></table>

**The buttons available on the screen:**\
The screen includes a set of buttons that allow the user to perform the following basic operations:

<table data-header-hidden><thead><tr><th valign="top">Button</th><th valign="top">Function</th></tr></thead><tbody><tr><td valign="top"><div><figure><img src="../../../../.gitbook/assets/image (508).png" alt=""><figcaption></figcaption></figure></div></td><td valign="top">When pressed, the system creates a new document to begin data entry.</td></tr><tr><td valign="top"><div><figure><img src="../../../../.gitbook/assets/image (504).png" alt=""><figcaption></figcaption></figure></div></td><td valign="top">Used to save the data entered or modified in the current document within the system.</td></tr><tr><td valign="top"><div><figure><img src="../../../../.gitbook/assets/image (505).png" alt=""><figcaption></figcaption></figure></div></td><td valign="top">Cancels the entry of new data or unsaved modifications and returns to the main screen without applying any changes.</td></tr><tr><td valign="top"><div><figure><img src="../../../../.gitbook/assets/image (506).png" alt=""><figcaption></figcaption></figure></div></td><td valign="top">Used to delete the selected record from the system, with confirmation required before final deletion to prevent accidental removal.</td></tr><tr><td valign="top"><div><figure><img src="../../../../.gitbook/assets/image (507).png" alt=""><figcaption></figcaption></figure></div></td><td valign="top">Allows printing of the current document or report according to the system’s approved print format.</td></tr></tbody></table>

**Example:**\
A company receives several post-dated cheques from a customer for a project payment. The accountant records them in the **Post-Dated Cheques Wallet** as follows:

* **Wallet Number:** PDC-2025-014
* **Wallet Date:** 14/10/2025
* **Bank Name:** National Bank of Egypt
* **Number of Cheques:** 3
* **Notes:** Cheques received for Project X payments

In the details grid below, the accountant enters:

| Receivable Note Number | Cheque Number | Customer Name | Currency | Total Amount | Due Date   | Deposited |
| ---------------------- | ------------- | ------------- | -------- | ------------ | ---------- | --------- |
| RN-00123               | 123456        | Al Noor Co.   | EGP      | 50,000       | 01/11/2025 | ☐         |
| RN-00124               | 123457        | Al Noor Co.   | EGP      | 50,000       | 15/11/2025 | ☐         |
| RN-00125               | 123458        | Al Noor Co.   | EGP      | 50,000       | 30/11/2025 | ☐         |

The **Total Amount** field at the top automatically displays **150,000 EGP**, representing the sum of all cheques.

Once each cheque reaches its **due date**, the accountant can mark it as **Deposited**, which updates the cheque’s status in the system for tracking and financial reporting.

