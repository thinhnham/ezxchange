<b>Synopsis

Ezxchange is a simple currency convert that will retreive exchange rates from Yahoo Finance. The program can be used on all devices (smart phones, tablets, and PCs). 

::Motivation

This web application was built with an intention to help travelers get an exchange rate easily for their trips 


::API Reference

Data is retreive from Yahoo Finance Exchange Rate API:

yql_query = 'select%20*%20from%20yahoo.finance.xchange%20where%20pair%20in%20("'+currencies1+currencies2+'")';
yql_query_url = yql_base_url + "?q=" + yql_query + "&format=json&env=store%3A%2F%2Fdatatables.org%2Falltableswithkeys";

Use an  ajax call (XMLHttpRequest/$.ajax()/$.get()) to send this query to Yahoo!

::Contributors

This program is simple. I'd like to add a graph that shows the periodic trend for the exchange rates. However, Yahoo Finance API doesn't have an API for the historical exchange rates.
They do have one but it has US Dollas as the base currency ! APIs for historical rates are not free. If anyone has access to historical rates, please expand this app. 

::License

(Apache, Javascript, BootstrapFormHelper, Jquery)
