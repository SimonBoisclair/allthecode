Create a 

At the `/` path, the HTTP response should have a content type of `text/html` and the body should be the following:

```html
<html>
    <body>
        <div id='somediv'></div>
        <script src='/somescript.js'></script>
    </body>
</html>
```

At the /somescript.js path, the HTTP response should be of type `application/javascript` and the body should be the following:

```javascript
document.getElementById("somediv").innerText="success!";
```


##Submission
Modify the file template.js directly.

Furthermore, take a screenshot of the webpage and put it in the submission folder.
