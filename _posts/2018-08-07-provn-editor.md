---
layout: post
title: ACE Editor for PROVN
---
The presented editor integrates [ACE editor](https://ace.c9.io/) with custom syntax highlighting and syntax validation using [ANTLR4](http://www.antlr.org/) grammar for [PROV-N](https://github.com/antlr/grammars-v4/tree/master/prov-n).

![PROV-N editor screenshot](https://raw.githubusercontent.com/h2020-westlife-eu/prov-n-editor/master/Editor1.PNG)

[PROV-N](https://www.w3.org/TR/2013/REC-prov-n-20130430/) is standard notation to hold provenance of data part of recomendation of [W3C PROV-O Ontology](https://www.w3.org/TR/prov-o/). 

The proof of concept sample editor can
- communicate with other web apps using cross document messaging API (window.opener.postMessage()).
- be filled by initial content using hash parameter 
  - 'content' for plain/text e.g.: https://h2020-westlife-eu.github.io/prov-n-editor/#content=document%0Dentity(e1)%0DendDocument
  - 'contentBase64' for base64 encoded text 
  - 'contentLZ' for LZ compressed and base64 encoded text,

![PROV-N editor screenshot](https://raw.githubusercontent.com/h2020-westlife-eu/prov-n-editor/master/Editor1.PNG)

## Live demo 
- [h2020-westlife-eu.github.io/prov-n-editor/](https://h2020-westlife-eu.github.io/prov-n-editor/)
- [Empty document](https://h2020-westlife-eu.github.io/prov-n-editor/)
- [short document](https://h2020-westlife-eu.github.io/prov-n-editor/#content=document%0Dentity(e1)%0DendDocument)
- [longer document encoded base64](https://h2020-westlife-eu.github.io/prov-n-editor/#contentBase64=ZG9jdW1lbnQNCiAgZGVmYXVsdCA8aHR0cDovL2Fub3RoZXJleGFtcGxlLm9yZy8+DQogIHByZWZpeCBleCA8aHR0cDovL2V4YW1wbGUub3JnLz4NCiAgZW50aXR5KGUyLCBbIHByb3Y6dHlwZT0iRmlsZSIsIGV4OnBhdGg9Ii9zaGFyZWQvY3JpbWUudHh0IiwgZXg6Y3JlYXRvcj0iQWxpY2UiLCANCiAgICAgICAgICAgICAgIGV4OmNvbnRlbnQ9IlRoZXJlIHdhcyBhIGxvdCBvZiBjcmltZSBpbiBMb25kb24gbGFzdCBtb250aC4iXSkNCiAgICAgICAgICAgICAgIGFjdGl2aXR5KGExLCAyMDExLTExLTE2VDE2OjA1OjAwLCAtLCBbcHJvdjp0eXBlPSJlZGl0Il0pDQogIHdhc0dlbmVyYXRlZEJ5KGUyLCBhMSwgLSwgW2V4OmZjdD0ic2F2ZSJdKSAgICAgDQogIHdhc0Fzc29jaWF0ZWRXaXRoKGExLCBhZzIsIC0sIFtwcm92OnJvbGU9ImF1dGhvciJdKQ0KICBhZ2VudChhZzIsIFsgcHJvdjp0eXBlPSdwcm92OlBlcnNvbicsIGV4Om5hbWU9IkJvYiIgXSkNCmVuZERvY3VtZW50)

## Source code
- https://github.com/h2020-westlife-eu/prov-n-editor
