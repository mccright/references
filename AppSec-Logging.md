Application Logging
===================

***Logging the NISTy Way***
 * Log all information that would be important for identifying the source or nature of an attack, or determining if an action is safe. [CWE-223](https://cwe.mitre.org/data/definitions/223.html)  
 * Log all authentication activities [CWE-778](https://cwe.mitre.org/data/definitions/778.html)  
 * Log all elevated-rights activity [CWE-778](https://cwe.mitre.org/data/definitions/778.html)  
 * Log all elevated-rights permission or access control changes [CWE-778](https://cwe.mitre.org/data/definitions/778.html)  
 * Log administrative activities [CWE-778](https://cwe.mitre.org/data/definitions/778.html)  
 * Log all access to sensitive data [CWE-778](https://cwe.mitre.org/data/definitions/778.html)  
 * Log only data that meets your risk tolerance [CWE-532](https://cwe.mitre.org/data/definitions/532.html)  
 * Log only enough to support application debugging, as well as recovery efforts or forensic analysis after an attack [CWE-779](https://cwe.mitre.org/data/definitions/779.html)  
 * Do not write secrets into the log files [CWE-532](https://cwe.mitre.org/data/definitions/532.html)  
 * When sensitive or critical information are required, encrypt them before logging [CWE-311](https://cwe.mitre.org/data/definitions/311.html)  
 * Logs are sensitive, protect them [CWE-533](https://cwe.mitre.org/data/definitions/533.html)  
 * Set log levels appropriately before promoting or shipping a product so that sensitive data and system information are not accidentally exposed to hostile agents. [CWE-532](https://cwe.mitre.org/data/definitions/532.html)  
 * Protect log files against unauthorized read/write. [CWE-532](https://cwe.mitre.org/data/definitions/532.html)  
 * Log only "safe" data {logs are an attack path, neutralize hostile content} [CWE-117](https://cwe.mitre.org/data/definitions/117.html)  
 * All error message text should be HTML entity encoded before being written to the log file to protect against potential cross-site scripting attacks against the viewer of the logs {logs are an attack path, neutralize hostile content} [CWE-497](https://cwe.mitre.org/data/definitions/497.html)  
 * Log only "known good" input.  Assume all input is malicious. Use a whitelist of acceptable inputs that strictly conform to specifications. Reject any input that does not strictly conform to specifications, or transform it into something that does.  

***Error Handling***
 * Display generic, non-descriptive error messages.  Where risk-appropriate, provide user guidance [CWE-209](https://cwe.mitre.org/data/definitions/209.html)  
 * Never emit unhandled errors [CWE-391](https://cwe.mitre.org/data/definitions/391.html)  
 * Configure an 'error-handler of last resort' [CWE-391](https://cwe.mitre.org/data/definitions/391.html)  
 * Suppress raw framework-generated errors [CWE-209](https://cwe.mitre.org/data/definitions/209.html)  
 * [CWE-]()  
 * [CWE-]()  
 * []()  
 * []()  
 * []()  
 

***NIST Guidance for Logging***  
*NIST SP 800-53 rev 4*  
**NIST AU-1  Audit Generation / System-Wide / Time-Correlated Audit Trail**  
The organization must have documented policies and procedures which establish an effective implementation of selected security controls related to auditing and accountability which are developed, disseminated, reviewed, and updated.  

**NIST AU-2   Audit and Accountability / Auditable Events**  
The organization must have a set of defined and auditable events and the captured information must be coordinated throughout the organization. An event is any observable occurrence in an organizational information system.  
Auditing requirements, including the need for auditable events, may be referenced in other security controls and control enhancements. Organizations also include auditable events that are required by applicable laws, regulations, directives, contracts, policies, and standards.  
Audit records can be generated at various levels of abstraction. Selecting the appropriate level of abstraction is a critical aspect of an audit capability and can facilitate the identification of root causes to problems.  
****List of Auditable Events:****  
a) Server alerts and error messages;  
b) User log-on and log-off (successful or unsuccessful);  
c) All system administration activities;  
d) Modification of privileges and access;  
e) Application start up and shut down;  
f) Application modifications (e.g., new code);  
g) Application alerts and error messages;  
h) Configuration changes;  
i) Account creation, modification, or deletion;  
j) File creation and deletion;  
k) Read access to information deemed critically sensitive (as prioritized by our various constituencies);  
l) Modification to information deemed critically sensitive (as prioritized by our various constituencies);  
m) Printing sensitive information; and  
n) Database modifications (e.g., schema changes, dropped tables, etc.);  
o) Any event or condition that is not specifically defined  

**NIST AU-3**  
Log records must contain information that establishes what type of event occurred, when the event occurred, where the event occurred, the source of the event, the outcome of the event, and the identity of any individuals or subjects associated with the event.  

**NIST AU-4**  
The organization must allocate audit record storage capacity consistent with necessary requirements laid out in current logging obligations.  

**NIST AU-5**  
The information system may, when shut down, overwrite the oldest audit records, or stop generating records during a process failure – consistent with its logging obligations.  

**NIST AU-6**  
The organization must regularly review information system audit records for inappropriate or unusual activities.  Reports of these audits must be generated and maintained.  

**NIST AU-7**  
The information system incorporates an approved audit reduction and report generation capability that supports on-demand audit review, analysis, and reporting requirements, after-the-fact investigations of security incidents.  This functionality must not alter the original content or time order of audit records.  

**NIST AU-8**  
The information system uses an internal system of clocks to generate audit record time stamps which are mapped to Coordinated Universal Time (UTC) or Greenwich Mean Time (GMT) and are/remain accurate-enough to meet all applicable laws, regulations, directives, contracts, policies, and standards.  

**NIST AU-9**  
The information system must effectively protect audit information and tools from unauthorized access, modification, and deletion.  

**NIST AU-11**  
The organization must retain audit records for the period of time defined by their formal records retention schedule to provide support for after-the-fact investigations of security incidents and to meet regulatory and company information retention requirements.  

**NIST AU-12 Audit Generation**  
The information system must have the capability to provide and generate audit records.  

**AU-12 (1) Audit Generation / System-Wide / Time-Correlated Audit Trail**  
The information system compiles audit records into a system-wide (logical or physical) audit trail that is time-correlated to within an organization-defined level of tolerance for relationship between time stamps of individual records in the audit trail.  

**AU-12 (2)	Audit Generation / Standardized Formats**  
The information system must have the capability to provide and generate audit records in Standardized Format(s).  


***Logging the OWASP Way***
 * Use their excellent CheatSheet: [https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Logging_Cheat_Sheet.md](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Logging_Cheat_Sheet.md)  


***Logging the GCHQ Way***
TODO: [https://github.com/gchq/event-logging](https://github.com/gchq/event-logging) and [https://github.com/gchq/event-logging-schema](https://github.com/gchq/event-logging-schema)  


**Log records should include at least the following elements:**  

* Identifier of the system that generated the event  
* Timestamp of the event  
* The action or type of event and any relevant data  
  * Additional context where relevant  
* Success or failure of the action  
* The user associated with the event  
* Remote address, if the event occurs over a network connection  
  * If there is a proxy or gateway in the path, pay special care to log the user's/the far endpoint's IP address, not the proxy/gateway.  
* (*selectively*) The browser user agent string, if the event occurs as the result of events initiated in/by a browser.  


***References***
 * Thank you SANS for sending a large paper poster on this topic to goose me into starting on this page.  SANS Securing Web Application Technologies (SWAT) checklist poster, received via surface mail 06-17-2019.  The initial entries in this list were from the top left corner of the checklist side of the poster.  
 * Common Weakness Enumeration (CWE™) List [https://cwe.mitre.org/data/index.html](https://cwe.mitre.org/data/index.html)
 * [http://www.cvedetails.com/cwe-definitions.php](http://www.cvedetails.com/cwe-definitions.php)  
 * Event Logging is an XML Schema for describing the auditable events generated by computer systems, hardware devices and access control systems. **Do not overlook this rich resource.** [https://gchq.github.io/event-logging-schema/](https://gchq.github.io/event-logging-schema/), and [https://github.com/gchq/event-logging-schema](https://github.com/gchq/event-logging-schema) with special emphasis on [https://gchq.github.io/event-logging-schema/basicStructure/#schema-uplift](https://gchq.github.io/event-logging-schema/basicStructure/#schema-uplift)  
 
