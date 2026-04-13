# Ready-Mix

<figure><img src="../../../.gitbook/assets/Gantt Chart Roadmap Whiteboard in Green Black Purple Sleek Digitalism Style.jpg" alt=""><figcaption></figcaption></figure>

### Bill of Material (BOM)

In AccFlex, the Bill of Materials (BOM) specifies the exact recipe for each concrete grade. When a customer places an order, the system instantly calculates how much cement, sand, and other materials are needed based on the BOM and the ordered quantity. Once the delivery plan status is "on the way," the system determines the required materials and automatically deducts them from inventory stock, and it's ready for mixing.

<figure><img src="../../../.gitbook/assets/BOM.gif" alt=""><figcaption><p>BOM</p></figcaption></figure>

### Ready-Mix Delivery

The **delivery planning** step takes place after the **sales order** and **bill of material** have been created. Information from the sales order is automatically populated into the delivery plan screen. After assigning the truck, driver, and assistant, the status of the delivery is selected. If the status is marked as **"On Way,"** the system automatically generates a goods issue. When the status is **“Delivered,”** the system creates the journal entry for the delivery, and at that point, the invoice can be created manually.

In cases where the delivery is **“Rejected** and **Destroyed,”** a scrap journal entry is created. If the goods are “rejected and directed to another customer,” the system creates a new sales order or updates an old sales order to the new customer. This process ensures that all delivery movements, rejections, and adjustments are accurately tracked and documented.

<figure><img src="../../../.gitbook/assets/Ready-Mix (not start).gif" alt=""><figcaption><p>Ready-Mix (not start)</p></figcaption></figure>

In conclusion, there are 4 case scenarios for the ready mix:

1\. **In Progress (On Way)**\
For concrete that has been in production under a manufacturing state, it generates a journal entry for the goods issue.

<figure><img src="../../../.gitbook/assets/Ready-Mix (On Way).gif" alt=""><figcaption><p>Ready-Mix (On Way)</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/good issue &#x26; journal (on Way).gif" alt=""><figcaption><p>good issue &#x26; journal (on Way)</p></figcaption></figure>

2\. **Delivered** \
When the customer formally accepts the delivery of the ready-mix, AccFlex automatically.

<figure><img src="../../../.gitbook/assets/Ready Mix (delivered).gif" alt=""><figcaption><p>Ready Mix (delivered)</p></figcaption></figure>

3\. **Redirection** \
When concrete needs to be redirected to a different project or customer, AccFlex adjusts the original sales order or creates a new one and reallocates inventory.

<figure><img src="../../../.gitbook/assets/Ready-Mix (rejected and redirected).gif" alt=""><figcaption><p>Ready-Mix (rejected and redirected)</p></figcaption></figure>

4\. **Rejected** \
In cases where the customer rejects the delivery due to quality issues, timing problems, or other reasons.

<figure><img src="../../../.gitbook/assets/Ready-Mix (Rejected and Destory).gif" alt=""><figcaption><p>Ready-Mix (Rejected and Destory)</p></figcaption></figure>

Each scenario maintains auditability while properly reflecting the financial impact in the appropriate accounting period, whether through revenue recognition, production under manufacturing, order modification, or loss recognition. The system's tight integration between operations and finance provides real-time visibility into both physical material movements and their corresponding financial effects.

{% hint style="info" %}
Hint: The delivery plan can be divided into multiple deliveries; this may happen due to truck capacity limits, scheduling constraints, or customer requirements. Each delivery created from the plan will have its own assigned truck, driver, and delivery status while still being linked to the original sales order.
{% endhint %}

**Journal Entries**

a.      Delivered

<table data-header-hidden><thead><tr><th valign="top"></th><th valign="top"></th><th valign="top"></th></tr></thead><tbody><tr><td valign="top">Description</td><td valign="top">Debit</td><td valign="top">Credit</td></tr><tr><td valign="top">Cogs</td><td valign="top">××</td><td valign="top"> </td></tr><tr><td valign="top">      Production under     Manufacture</td><td valign="top"> </td><td valign="top">××</td></tr></tbody></table>

b.     In progress

<table data-header-hidden><thead><tr><th valign="top"></th><th valign="top"></th><th valign="top"></th></tr></thead><tbody><tr><td valign="top">Description</td><td valign="top">Debit</td><td valign="top">Credit</td></tr><tr><td valign="top">Production under Manufacture</td><td valign="top">××</td><td valign="top"> </td></tr><tr><td valign="top">     Stock</td><td valign="top"> </td><td valign="top">××</td></tr></tbody></table>

c. Rejected

<table data-header-hidden><thead><tr><th valign="top"></th><th valign="top"></th><th valign="top"></th></tr></thead><tbody><tr><td valign="top">Description</td><td valign="top">Debit</td><td valign="top">Credit</td></tr><tr><td valign="top">Scrap Expense</td><td valign="top">××</td><td valign="top"> </td></tr><tr><td valign="top">      Production under Manufacture</td><td valign="top"> </td><td valign="top">××</td></tr></tbody></table>
