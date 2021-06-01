# GET aHEAD
Replaced **GET** request (from red button) with **HEAD**, as a result flag is returned!

# Cookies
First a **POST** request is generated from search button, just let it go. Then, a **GET** request is generated which has hearder named **"Cookies"**, it has name key whose value is an integer. Just keep increasing that integer and analyze the response. On `name=18` it returned the flag.

# Insp3ct0r
Simple!
flag is divided in 3 parts

 1. comment in **.html** file
 2. comment in **strong text**

<!--stackedit_data:
eyJoaXN0b3J5IjpbMzc0NjM3MjM1XX0=
-->