# GET aHEAD
Replaced **GET** request (from red button) with **HEAD**, as a result flag is returned!

# Cookies
First a **POST** request is generated from search button, just let it go. Then, a **GET** request is generated which has hearder named **"Cookies"**, it has name key whose value is an integer. Just keep increasing that integer and analyze the response. On `name=18` it returned the flag.

# Insp3ct0r
**Flag :** picoCTF{tru3_d3t3ct1ve_0r_ju5t_lucky?832b0699}

Simple!
flag is divided in 3 parts

 1. comment in **.html** file
 2. comment in **.css** file
 3. comment in **.js** file

# Scavenger Hunt
**Flag :** picoCTF{th4ts_4_l0t_0f_pl4c
A bit complicated that previous one
again flag is divided in ** parts** :

 1. comment in **html**  file
 2. comment in **css** file
 3. comment in js shows about controling index which relates to **robots.txt** file. So get **robots.txt** using a **GET** request which somes next hint :<br /> `I think this is an apache server... can you Access the next flag?`
 4. 

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTg3NTQ0OTE3MCw5MjUyMDc3NzMsMTU3NT
E2OTkyNl19
-->