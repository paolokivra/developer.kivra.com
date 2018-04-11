# Partner API

The Partner API allows authorized partners to access and retrieve documents from the kivra inbox of companies. 
This is typically done to allow for further processing of the documents like for instance bookkeeping.

A company must explicitly provide a partner with the right to access its documents, by switching on a corresponding option 
in the settings page of the company in Kivra. Once a company has allowed a partner to retrieve the documents, the partner can 
start retrieving documents, even those that a company received before enabling the access to the partner.

A company can at any time stop providing access to a partner by switching off the corresponding options in the setting 
page of the company in Kivra. 

## Typical process

1. Company C is using software S made by P, a Partner of Kivra
2. Company C chooses to activate the connection between Software S and Kivra. Software S may start polling Kivra 
using the partner API to retrieve documents, however this will not work until nest step is completed.
3. Company C logs in to Kivra and switches on permission to access documents for Software S, using the Settings page of Kivra 
4. At this point when Software S tries to retrieve documents for Company C using the Partner API, it will receive a 
positive response.
5. Software S can now access and process documents for Company C

## API process

1. Each customer wanting to access the partner API needs to have authorised Client ID / Client Secret credentials. 
2. The client credentials are used to retrieve an access token with a specific scope allowing to retrieve documents 
for one specific company.
3. 
