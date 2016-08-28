# Blockchain_info_WHMCS_Payment_Gateway
Blockchain.info WHMCS Payment Gateway  This is a payment gateway that integrates Blockchain.info's Receiving API with WHMCS.  Blockchain.info's receiving API offers free Bitcoin transactions of 0.0005 BTC or greater. No account is required. To install, simply upload the necessary files and configure your Bitcoin address where you wish to receive payments.  When a customer selects Blockchain.info as their payment gateway on the invoice page, the gateway contacts Blockchain.info requesting the current conversion rate in your currency, and a fresh Bitcoin address. The price in BTC is only requested once and is stored, even if the customer closes the invoice and comes back to it later. This prevents the cost of a transaction from fluctuating depending on the current market status. Once the customer sends a payment to the address listed on the invoice, the page will update live with the payment's status. If you choose to make the client wait for a specific number of confirmations, the invoice will display how many confirmations have been received and how many are required. Once enough confirmations are received, the invoice will be updated to Paid status and the page will be refreshed.  You may wish to update the gateway's display name from "Blockchain.info" to "Bitcoin" for the sake of clarity for your customers.  If you wish to donate for this module, you may donate to  1FmKDpq9Ez5HHT1uh1RJitwbwdg5PR59W3   Installation  Download the latest release, extract it, and upload the modules folder contained in the zip to your WHMCS root directory. Then enter your WHMCS admin panel, and navigate to Setup > Payments > Payment Gateways. In the Activate Module dropdown, select Blockchain.info and click Activate. Finally, in the Blockchain.info section, fill in your desired display name for the module on invoices, your Bitcoin address, and how many confirmations you want to require for an invoice to be marked Paid. To accept transactions immediately without waiting for confirmations, you can leave the "Confirmations Required" field blank.
