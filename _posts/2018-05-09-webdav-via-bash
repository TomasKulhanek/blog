---
layout: post
title: WEBDAV via bash
---
## WEBDAV via bash
[Web Distributed Authoring and Versioning (WebDAV)](https://en.wikipedia.org/wiki/WebDAV) is extension of HTTP. Thus HTTP requests can be used in order to GET or PUT file.
Prerequisite: install curl using your OS package manager `yum install curl` or `apt-get install curl`. cURL is command-line tool for transferring data using various protocols available as standard package in most OS.

Bash script to UPLOAD file to the webdav URL (note PUT request may not be allowed by generic web site or may need further authentication)

```bash
curl -X PUT [updirurl+filename] --data "any text content"
```

Bash script to DOWNLOAD file from the webdav URL

```bash
curl [updirurl+filename] --data "any text content"
```

[Download full sample script](https://gist.github.com/TomasKulhanek/c94e148159a871ee688685828da82ebd)
