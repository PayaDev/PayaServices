**Input**:  
 - Paya Services Merchant ID as Integer
 - Accepts an XML string called a data packet that must conform to the new terminal application schema.
    
**Output**:  
- Outputs an XML string.

# SOAP 1.1
## Request:
**Header Information:**  
POST /webservices/AppGateway.asmx HTTP/1.1  
Host: demo.eftchecks.com  
Content-Type: text/xml; charset=utf-8  
Content-Length: length  
SOAPAction: "http://tempuri.org/GETI.eMagnus.WebServices/AppGateway/BoardCertificationLocation_Check21"



```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <RemoteAccessHeader xmlns="http://tempuri.org/GETI.eMagnus.WebServices/AppGateway">
      <UserName>string</UserName>
      <Password>string</Password>
      <TerminalID>int</TerminalID>
    </RemoteAccessHeader>
  </soap:Header>
  <soap:Body>
    <BoardCertificationLocation_Check21 xmlns="http://tempuri.org/GETI.eMagnus.WebServices/AppGateway">
      <merchantID>int</merchantID>
      <DataPacket>string</DataPacket>
    </BoardCertificationLocation_Check21>
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
    <BoardCertificationLocation_Check21Response xmlns="http://tempuri.org/GETI.eMagnus.WebServices/AppGateway">
      <BoardCertificationLocation_Check21Result>string</BoardCertificationLocation_Check21Result>
    </BoardCertificationLocation_Check21Response>
  </soap:Body>
</soap:Envelope>
```

# SOAP 1.2

## Request:
**Header Information:**  
POST /webservices/AppGateway.asmx HTTP/1.1  
Host: demo.eftchecks.com  
Content-Type: application/soap+xml; charset=utf-8  
Content-Length: length  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap12:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap12="http://www.w3.org/2003/05/soap-envelope">
  <soap12:Header>
    <RemoteAccessHeader xmlns="http://tempuri.org/GETI.eMagnus.WebServices/AppGateway">
      <UserName>string</UserName>
      <Password>string</Password>
      <TerminalID>int</TerminalID>
    </RemoteAccessHeader>
  </soap12:Header>
  <soap12:Body>
    <BoardCertificationLocation_Check21 xmlns="http://tempuri.org/GETI.eMagnus.WebServices/AppGateway">
      <merchantID>int</merchantID>
      <DataPacket>string</DataPacket>
    </BoardCertificationLocation_Check21>
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
    <BoardCertificationLocation_Check21Response xmlns="http://tempuri.org/GETI.eMagnus.WebServices/AppGateway">
      <BoardCertificationLocation_Check21Result>string</BoardCertificationLocation_Check21Result>
    </BoardCertificationLocation_Check21Response>
  </soap12:Body>
</soap12:Envelope>
```

