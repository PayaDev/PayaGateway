
![Paya_Exchange_Virtual_Desktop_Logo](https://user-images.githubusercontent.com/6975101/191064534-ddc55561-7530-4b1c-9765-232a363b1e91.jpeg)



![Paya_Exchange_Virtual_Desktop](https://user-images.githubusercontent.com/6975101/182176143-eb9c4f97-bbc4-4c36-97ad-19fac890c19a.png)


# Paya Exchange Virtual Desktop (PEVD)

 
PEVD GitHub sample repo and documentation - [https://github.com/PayaDev/PayaGateway/tree/master/PayaCore/Paya-Exchange-Virtual-Desktop
](https://github.com/PayaDev/PayaGateway/tree/master/PayaCore/Paya-Exchange-Virtual-Desktop)
PEVD operates as a redirect. We do not support PEVD within an iframe. You create an XML request a and submit using an html Form POST.
 
## Server Side Operation:
**Build Request Envelope** - https://www.sageexchange.com/sevd/frmenvelope.aspx

This endpoint will allow you to submit your initial unencoded XML request and returns an encoded envelope. 

## Client Side Operation:
**Submit Payment Request Envelope** - https://www.sageexchange.com/sevd/frmpayment.aspx

This endpoint will allow you to submit your encoded envelope to initiate the payment or vault form. When your user completes their interaction with the form PEVD will return an encoded response envelope.

## Server Side Operation:
**Open Response Envelope** - https://www.sageexchange.com/sevd/frmopenenvelope.aspx

This endpoint will allow you to submit your encoded response envelope and returns the unencoded XML for your consumption. The data is returned to your redirect or through a postback if you include a postback URL.

