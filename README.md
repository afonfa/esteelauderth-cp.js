<script type="text/javascript" data="olapic-checkout">
//==== Olapic Require: DO NOT CHANGE
var olapicRequireCheckoutScript=(function(oHead){var onError=function(){throw new URIError('Olapic checkout script could not be loaded');};return function(olapicScriptSrc,onLoadCallback){var oScript=document.createElement('script');oScript.type='text\/javascript';oScript.src=olapicScriptSrc;oScript.async=true;oScript.onerror=onError;if(onLoadCallback){if(oScript.addEventListener){oScript.addEventListener('load',onLoadCallback,false);}else if(oScript.readyState){oScript.onreadystatechange=function(){if(!this.readyState||this.readyState==='loaded'||this.readyState==='complete'){onLoadCallback();}};}else{oScript.attachEvent('load',onLoadCallback);}}
oHead.appendChild(oScript);};})(document.head||document.getElementsByTagName('head')[0]);

// ==== Checkout Code:
olapicRequireCheckoutScript('//photorankstatics-a.akamaihd.net/static/frontend/checkout/olapic.checkout.helper.js', function(){
    // Initialization
    olapicCheckout.init('c19cd51027cb401b64bafa529ed8d04198cce2975fbb9aee373496f70c3b4a4b');

    // Add the Products: Product loop starts. This is where you will store each product purchased info
    olapicCheckout.addProduct('PRODUCT_ID', PRODUCT_PRICE);
    // Product loop ends.

    // Add the metadata/attributes
    olapicCheckout.addAttribute('transactionId', 'TRANSACTION_ID');
    olapicCheckout.addAttribute('currencyCode', 'CURRENCY');
    // Add Segmentation Values
    olapicCheckout.addSegment('SEGMENT_KEY', 'SEGMENT_VALUE');
    // Send the information
    olapicCheckout.execute();
});
</script>
