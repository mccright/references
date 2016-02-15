Application Logging
===================

***Logging***
 * Log all authentication activities [CWE-778](https://cwe.mitre.org/data/definitions/778.html)  
 * Log all elevated-rights activity [CWE-778](https://cwe.mitre.org/data/definitions/778.html)  
 * Log all elevated-rights changes [CWE-778](https://cwe.mitre.org/data/definitions/778.html)  
 * Log administrative activities [CWE-778](https://cwe.mitre.org/data/definitions/778.html)  
 * Log all access to sensitive data [CWE-778](https://cwe.mitre.org/data/definitions/778.html)  
 * Log only data that meets your risk tolerance [CWE-532](https://cwe.mitre.org/data/definitions/532.html)  
 * Do not write secrets into the log files. [CWE-532](https://cwe.mitre.org/data/definitions/532.html)  
 * Logs are sensitive, protect them [CWE-533](https://cwe.mitre.org/data/definitions/533.html)  
 * Set log levels appropriately before promoting or shipping a product so that sensitive data and system information are not accidentally exposed to hostile agents. [CWE-532](https://cwe.mitre.org/data/definitions/532.html)  
 * Protect log files against unauthorized read/write. [CWE-532](https://cwe.mitre.org/data/definitions/532.html)  
 * Log only "safe" data {logs are an attack path, neutralize hostile content} [CWE-117](https://cwe.mitre.org/data/definitions/117.html)  
 * Log only "known good" input.  Assume all input is malicious. Use a whitelist of acceptable inputs that strictly conform to specifications. Reject any input that does not strictly conform to specifications, or transform it into something that does.


***Error Handling***
 * Display generic, non-descriptive error messages [CWE-209]()  
 * Never emit unhandled errors [CWE-391]()  
 * Configure an 'error-handler of last resort' [CWE-391]()  
 * Suppress framework-generated errors [CWE-209]()  
 * [CWE-]()  
 * [CWE-]()  
 * []()  
 * []()  
 * []()  
 * []()  
 * []()  
 * []()  

***References***
 * Thank you SANS for sending a large paper poster on this topic to goose me into starting on this page.  SANS Securing Web Application Technologies (SWAT) checklist poster, received via surface mail 06-17-2019.  The initial entries in this list were from the top left corner of the checklist side of the poster.  
 * Common Weakness Enumeration (CWE™) List [https://cwe.mitre.org/data/index.html](https://cwe.mitre.org/data/index.html)
 * [http://www.cvedetails.com/cwe-definitions.php](http://www.cvedetails.com/cwe-definitions.php)  
