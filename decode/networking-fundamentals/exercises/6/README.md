Write a function that checks cnn.com to see if they're talking about trump. It console logs "trump news today" if cnn.com is talking about trump, otherwise it console logs "no trump".
# Reference

You will need to use the `.indexOf` string method. Use it to see if the word trump appears anywhere in the HTML page.

Use the following as a starting point. The response will contain an HTML page.

```javascript
var net = require('net');
function makeRequest(addr, req, f) {
    var client = new net.Socket();
    client.connect(80, addr, function () {
        return client.write(req);
    });
    client.on("data", function (data) {
        f(data.toString());
    });
}

//The following string *MUST* end with 2 newlines
var http_request =
    `GET /index.html HTTP/1.1
host: www.dolekemp96.com

`;

makeRequest("www.dolekemp96.org", http_request, x => console.log(x))
```