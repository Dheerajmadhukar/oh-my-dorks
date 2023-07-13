# Google Dorks for Bug Bounty

A list of Google Dorks for Bug Bounty, Web Application Security, and Pentesting

[![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/Dheerajmadhukar.svg?style=social&label=Follow%20%40Dheerajmadhukar)](https://twitter.com/Dheerajmadhukar)
</p>

---

### Broad domain search w/ negative search

> site:example.com -www -shop -share -ir -mfa

### PHP extension w/ parameters

> site:"example.com" intext:"php" inurl:".php?id=" OR inurl:".php?param=" OR inurl:".php?file=" OR inurl:".php?query=" OR inurl:".php?category=" OR inurl:".php?search=" OR inurl:".php?keyword=" OR inurl:".php?name=" OR inurl:".php?var=" OR inurl:".php?value=" OR inurl:".php?type=" OR inurl:".php?code=" OR inurl:".php?item=" OR inurl:".php?section=" OR inurl:".php?option=" OR inurl:".php?view=" OR inurl:".php?data=" OR inurl:".php?content=" OR inurl:".php?lang=" OR inurl:".php?config=" OR inurl:".php?template=" OR inurl:".php?ref=" OR inurl:".php?target=" OR inurl:".php?url=" OR inurl:".php?redirect=" OR inurl:".php?return=" OR inurl:".php?link=" OR inurl:".php?site=" OR inurl:".php?url=" OR inurl:".php?go=" OR inurl:".php?out=" OR inurl:".php?view=" OR inurl:".php?dir=" OR inurl:".php?pg=" OR inurl:".php?req=" OR inurl:".php?document=" OR inurl:".php?func=" OR inurl:".php?cmd=" OR inurl:".php?action=" OR inurl:".php?func=" OR inurl:".php?load=" OR inurl:".php?exec=" OR inurl:".php?execute=" OR inurl:".php?query=" OR inurl:".php?process=" OR inurl:".php?do=" OR inurl:".php?func=" OR inurl:".php?read=" OR inurl:".php?include=" OR inurl:".php?config=" OR inurl:".php?load=" OR inurl:".php?execute="

### SSRF

> site:example.com (inurl:"?data=" OR inurl:"?data_uri=" OR inurl:"?data_url=" OR inurl:"?download=" OR inurl:"?download_url=" OR inurl:"?endpoint=" OR inurl:"?external=" OR inurl:"?external_link=" OR inurl:"?external_url=" OR inurl:"?fetch=" OR inurl:"?fetch_url=" OR inurl:"?file=" OR inurl:"?file_url=" OR inurl:"?forward=" OR inurl:"?forward_url=" OR inurl:"?image=" OR inurl:"?image_source=" OR inurl:"?image_url=" OR inurl:"?link=" OR inurl:"?load=" OR inurl:"?load_url=" OR inurl:"?navigate=" OR inurl:"?out=" OR inurl:"?path=" OR inurl:"?path_to_file=" OR inurl:"?proxy=" OR inurl:"?proxy_link=" OR inurl:"?proxy_url=" OR inurl:"?read=" OR inurl:"?redirect=" OR inurl:"?redirect_url=" OR inurl:"?remote=" OR inurl:"?remote_image=" OR inurl:"?remote_image_url=" OR inurl:"?remote_url=" OR inurl:"?request=" OR inurl:"?rurl=" OR inurl:"?source_url=" OR inurl:"?src=" OR inurl:"?target=" OR inurl:"?target_path=" OR inurl:"?target_uri=" OR inurl:"?target_url=" OR inurl:"?uri=" OR inurl:"?url=" OR inurl:"?url_path=" OR inurl:"?urlto=")

### Disclosed XSS and Open Redirects

> site:openbugbounty.org inurl:reports intext:"example.com"

### Juicy Extensions

> site:"example.com" -inurl:robots.txt -inurl:sitemap.xml ext:sql OR ext:db OR ext:conf OR ext:config OR ext:log OR ext:backup OR ext:old OR ext:bak OR ext:ini OR ext:env OR ext:htaccess OR ext:passwd OR ext:txt OR ext:csv OR ext:xml OR ext:json OR ext:yml OR ext:yaml OR ext:wp-config.php OR ext:db.inc OR ext:env.inc OR ext:config.inc OR ext:ini.inc OR ext:log.inc OR ext:backup.inc OR ext:sql.inc OR ext:conf.inc OR ext:htaccess.inc OR ext:passwd.inc OR ext:key.inc OR ext:txt.inc OR ext:bak.inc OR ext:xml.inc OR ext:csv.inc OR ext:pdf.inc OR ext:ppt.inc OR ext:pptx.inc OR ext:xls.inc OR ext:xlsx.inc OR ext:md OR ext:htm OR ext:html OR ext:phps OR ext:phtml OR ext:shtm OR ext:shtml OR ext:asp OR ext:aspx OR ext:pl OR ext:cgi OR ext:cfm OR ext:cfc OR ext:rb OR ext:py OR ext:java OR ext:sh OR ext:bat OR ext:cmd OR ext:asm OR ext:c OR ext:cpp OR ext:cs OR ext:swift OR ext:vb OR ext:pas OR ext:inc OR ext:css OR ext:scss OR ext:less OR ext:js OR ext:jsx OR ext:vue OR ext:ts OR ext:tsx OR ext:coffee OR ext:go OR ext:rs OR ext:hs OR ext:fs OR ext:erl OR ext:exs OR ext:ex OR ext:clj OR ext:lua OR ext:pl OR ext:pm OR ext:tcl OR ext:ml OR ext:fsx OR ext:fsi OR ext:fsproj OR ext:h OR ext:hpp OR ext:m OR ext:mm OR ext:groovy OR ext:kt OR ext:php4 OR ext:php3 OR ext:php2 OR ext:phtml OR ext:pwml OR ext:inc OR ext:php2 OR ext:inc.php

### Code Leaks

> site:pastebin.com "example.com"

> site:jsfiddle.net "example.com"

> site:codebeautify.org "example.com"

> site:codepen.io "example.com"

### Cloud Storage

> site:s3.amazonaws.com "example.com"

> site:blob.core.windows.net "example.com"

> site:googleapis.com "example.com"

> site:drive.google.com "example.com"

> site:dev.azure.com "example[.]com"

> site:onedrive.live.com "example[.]com"

> site:digitaloceanspaces.com "example[.]com"

> site:sharepoint.com "example[.]com"

> site:s3-external-1.amazonaws.com "example[.]com"

> site:s3.dualstack.us-east-1.amazonaws.com "example[.]com"

> site:dropbox.com/s "example[.]com"

> site:box.com/s "example[.]com"

> site:docs.google.com inurl:"/d/" "example[.]com"

### XSS prone parameters

> inurl:q= | inurl:s= | inurl:search= | inurl:query= inurl:& site:example.com

### Open Redirect prone parameters

> inurl:url= | inurl:return= | inurl:next= | inurl:redir= inurl:http site:example.com

### SQLi Prone Parameters

> inurl:id= | inurl:pid= | inurl:category= | inurl:cat= | inurl:action= | inurl:sid= | inurl:dir= inurl:& site:example.com

### SSRF Prone Parameters

> inurl:http | inurl:url= | inurl:path= | inurl:dest= | inurl:html= | inurl:data= | inurl:domain=  | inurl:page= inurl:& site:example.com

### LFI Prone Parameters

> inurl:include | inurl:dir | inurl:detail= | inurl:file= | inurl:folder= | inurl:inc= | inurl:locate= | inurl:doc= | inurl:conf= inurl:& site:example.com

### RCE Prone Parameters

> inurl:cmd | inurl:exec= | inurl:query= | inurl:code= | inurl:do= | inurl:run= | inurl:read=  | inurl:ping= inurl:& site:example.com

### High % inurl keywords

> inurl:config | inurl:env | inurl:setting | inurl:backup | inurl:admin | inurl:php site:example[.]com

### Sensitive Parameters

> inurl:email= | inurl:phone= | inurl:password= | inurl:secret= inurl:& site:example[.]com

### JFrog Artifactory

> site:jfrog.io "example[.]com"

### Firebase

> site:firebaseio.com "example[.]com"

### API Docs

> inurl:apidocs | inurl:api-docs | inurl:swagger | inurl:api-explorer site:"example[.]com"

### File upload endpoints

> site:example.com ”choose file”

## Dorks that work better w/o domain

### Bug Bounty programs and Vulnerability Disclosure Programs

> "submit vulnerability report" | "powered by bugcrowd" | "powered by hackerone"

> site:*/security.txt "bounty"

### Apache Server Status Exposed

> site:*/server-status apache

### WordPress

> inurl:/wp-admin/admin-ajax.php

### Drupal

> intext:"Powered by" & intext:Drupal & inurl:user

### Joomla

> site:*/joomla/login

---

