# API architectur documentation
this documentation is for OnBox private and public API, this document make first by Herman Sugiharto at 12th July 2018.

## Private API
Private API is only for OnBox Internal Application

*included file*

-------------
(success)[200] private/private__profil-page.json

### url request

`https://onbox.com/v1/!#/private/user/{{@user}}`

**@user**       : username of user (with @ in eginning)

*general purpose*
this API is to get all information and post for provil page

### return
[200] user information

*full documentation file*
private/private__profil-page.md

-----------

(failure)[400] private/private__profil-page-404.json


## Public API
Public API can be used by registered developer in developer.onbox.com
