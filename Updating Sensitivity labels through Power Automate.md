
Update File Properties action in SharePoint, available within Power Automate, allows you to modify metadata associated with files stored in document libraries.

![Uploading image.png…](https://github.com/AlmasMahfooz/NotWorking/blob/main/SP0.png)

But Update file properties don't provide a way to update any of the fields related to labels.
'OData__DisplayName' is the field name for Sensitivity data information, two other fields are Label ID Label Display Name.
Sensitivity/OData_DisplayName and SensitivityLabelName both contain the value of label, in this case it is "Internal".
"{SensitivityLabelId}": "ec7c3683-4e14-4efa-b36b-9868c5883c6f",
"{SensitivityLabelName}": "Internal"

![Uploading image.png…](https://github.com/AlmasMahfooz/NotWorking/blob/main/SP1.png)


Tried Send an HTTP request to SharePoint but it seems it doesn't recognize the label fields.
Header code

json('{"Accept":"application/json;odata=verbose","Content-Type":"application/json;odata=verbose","X-HTTP-Method":"MERGE","IF-MATCH":"*"}')



![Uploading image.png…](https://github.com/AlmasMahfooz/NotWorking/blob/main/SP2.png)









links:
https://learn.microsoft.com/en-us/sharepoint/dev/business-apps/power-automate/guidance/working-with-send-sp-http-request
![Uploading image.png…]
