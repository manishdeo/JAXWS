JAXWS
=====

Java with JAXWS

Request:
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ser="http://service.ws.jax.bank.com/">
   <soapenv:Header/>
   <soapenv:Body>
      <ser:bankDeposit>
         <!--Optional:-->
         <account>3344440044</account>
         <!--Optional:-->
         <amount>1520.00</amount>
         <!--Optional:-->
         <name>MANISH DEO</name>
      </ser:bankDeposit>
   </soapenv:Body>
</soapenv:Envelope>



Response

<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Body>
      <ns2:bankDepositResponse xmlns:ns2="http://service.ws.jax.bank.com/">
         <transaction>Your Transaction of Rs 1520.00 credited successfully!</transaction>
      </ns2:bankDepositResponse>
   </soap:Body>
</soap:Envelope>


