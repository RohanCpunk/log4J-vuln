What is log4J?

-"the single biggest most critical vulnerability of the decade"

-this vulnerabity allows an attacker to execute code on a remote server: a so-called RCE (Remote Code Execution)
-Reported to Apache by Alibaba on November 24,2021, and Published in a tweet on december 9 2021
-Affected services include "CloudeFlare,iCloud,Minecraft:java Edition, Steam , Tencent QQ, and Twitter
-Apache Software Foundation assinged the MAXIMUM CVSS severity rating of 10
-Technical Description :
    = In Apache log4j version up to and including 2.14.1(2.0 to 2.14.1, Excluding security release 2.12.2),
      The JNDI features used in configuration , log messages and parameters do not protect against attacker-controlled LDAP 
      and other JNDI related endpoints An attacker who can control log messages or log messages parametr can execute code loaded from LDAP servers
      when messages lookup substitution is enabled 

WHY LOGGING ? 

- can write to files and databases without and active console 
-log formation 
-error tracing and debugging
-incident tracking 
-log levels (info,error,