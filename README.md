# OWASP Unrestricted File Upload
Repo to help security enthusiasts while testing against unrestricted file upload & test upload of malicious files based on the [OWASP documentation][owasp-unreq-guide].

## Webshell

This module aims to reproduce a webshell creation attempt by an attacker.
It has the following levels of filter evasion:

| Level | Description |
| ------ | ------ |
| 1 | [Change the capitalisation of the extension][level-1] |
| 2 | [Change the extensions to a less common extension + Using special trailing characters such as spaces, dots or null characters][level-2] |
| 3 | [Level 2 + Additional extension, in case the server cares only about the last extension][level-3] |
| 4 | [The opposity logic of the 3rd level. It's used when the server cares only about the first extension in the file name.][level-4] |

[//]: # (Reference links)

   [owasp-unreq-guide]: <https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/10-Business_Logic_Testing/09-Test_Upload_of_Malicious_Files>
   [level-1]: <https://github.com/Att4ck3rS3cur1ty/Unrestricted-File-Upload/tree/master/webshell/level_1>
   [level-2]: <https://github.com/Att4ck3rS3cur1ty/Unrestricted-File-Upload/tree/master/webshell/level_2>
   [level-3]: <https://github.com/Att4ck3rS3cur1ty/Unrestricted-File-Upload/tree/master/webshell/level_3>
   [level-4]: <https://github.com/Att4ck3rS3cur1ty/Unrestricted-File-Upload/tree/master/webshell/level_4>