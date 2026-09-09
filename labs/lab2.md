## LAB 2 WRITEUP

 * vulnerability type   :- STORED XSS 
 * LAB TOPIC            :- STORED XSS INTO HTML CONTEXT WITH NOTHING ENCODED
  
 *  STEPS  
  
  1. Access  the lab and view & click the  blog post 
  2. after that in commect section use i nject malicious script <script>alert(1)</script>  , enter email id , website name    
  3. and press enter . observe the jsvascript execution 

 * IMPACT  :- The payload submitted through comment section . the application store the input in the server . when the user visit the affected page . then the script execute and user got affected . 
