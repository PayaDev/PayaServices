**Input**:  
- Accepts an XML string called a data packet that must conform to the terminals schema provided in the Terminal Settings.
- In addition to the fields for ProcessSingleCheck, this also allows control of voiding specific transactions via the TRANSACTION_ID and TRANSACTION_AUTH_NUMBER field.
  
**Output**:  
- Outputs an XML string.

# SOAP 1.1
## Request:
**Header Information:**  
POST /webservices/AuthGateway.asmx HTTP/1.1  
Host: demo.eftchecks.com  
Content-Type: text/xml; charset=utf-8  
Content-Length: length  
SOAPAction: "http://tempuri.org/GETI.eMagnus.WebServices/AuthGateway/ProcessSingleCheckAndGetTransAuthNum"


```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ProcessSingleCheckAndGetTransAuthNum xmlns="http://tempuri.org/GETI.eMagnus.WebServices/AuthGateway">
      <DataPacket>string</DataPacket>
    </ProcessSingleCheckAndGetTransAuthNum>
  </soap:Body>
</soap:Envelope>
```


## Response:
**Header Information:**  
HTTP/1.1 200 OK  
Content-Type: text/xml; charset=utf-8  
Content-Length: length  

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ProcessSingleCheckAndGetTransAuthNumResponse xmlns="http://tempuri.org/GETI.eMagnus.WebServices/AuthGateway">
      <ProcessSingleCheckAndGetTransAuthNumResult>string</ProcessSingleCheckAndGetTransAuthNumResult>
    </ProcessSingleCheckAndGetTransAuthNumResponse>
  </soap:Body>
</soap:Envelope>
```

# SOAP 1.2

## Request:
**Header Information:**  
POST /webservices/AuthGateway.asmx HTTP/1.1  
Host: demo.eftchecks.com  
Content-Type: application/soap+xml; charset=utf-8  
Content-Length: length  
 
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap12:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap12="http://www.w3.org/2003/05/soap-envelope">
  <soap12:Header>
    <AuthGatewayHeader xmlns="http://tempuri.org/GETI.eMagnus.WebServices/AuthGateway" />
  </soap12:Header>
  <soap12:Body>
    <ProcessSingleCheckAndGetTransAuthNum xmlns="http://tempuri.org/GETI.eMagnus.WebServices/AuthGateway">
      <DataPacket>string</DataPacket>
    </ProcessSingleCheckAndGetTransAuthNum>
  </soap12:Body>
</soap12:Envelope>
```

## Response:
**Header Information:**  
HTTP/1.1 200 OK  
Content-Type: text/xml; charset=utf-8  
Content-Length: length  

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap12:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap12="http://www.w3.org/2003/05/soap-envelope">
  <soap12:Body>
    <ProcessSingleCheckAndGetTransAuthNumResponse xmlns="http://tempuri.org/GETI.eMagnus.WebServices/AuthGateway">
      <ProcessSingleCheckAndGetTransAuthNumResult>string</ProcessSingleCheckAndGetTransAuthNumResult>
    </ProcessSingleCheckAndGetTransAuthNumResponse>
  </soap12:Body>
</soap12:Envelope>
```
