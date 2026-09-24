## LAB 3 WRITEUP

 * vulnerability type   :- DATA OBJECT MODEL XSS  (DOM)
 * LAB TOPIC            :- Exploiting DOM XSS with different sources and sinks
  
 *  STEPS  
  
  1. Access  the lab and view search bar  
  2. enter random alphanumeric string and press enter
  3. open developer mode and see on source tab under which LAB.JS were there 
  4. search to **location.search** 
  5. edit the url and add <img src=1 onerror=alert(1)></img>
  6. and press enter

 * IMPACT  :- The payload sent thorugh url parameter . the application check img src . img src failed . error generate and alert function() trigger . input goes to search tab 
   
   ![xss proof of concept ](image.png)