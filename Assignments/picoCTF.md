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
**Flag :** picoCTF{th4ts_4_l0t_0f_pl4c3s_2_lO0k_35844447}

A bit complicated that previous one
again flag is divided in **5 parts** :

 1. comment in **html**  file
 2. comment in **css** file
 3. comment in js shows about controling index which relates to **robots.txt** file. So get **robots.txt** using a **GET** request which somes next hint :<br /> `I think this is an apache server... can you Access the next flag?`
 4. apache server have **.htaccess** file. So, get it by **GET** request which gives next hint :<br />`I love making websites on my Mac, I can Store a lot of information there.`
 5. What stands out the most about that hint is the capitalized "Store". In Macs, a `.DS_Store`  file stores the configurations for how the desktop looks (eg. icon location, etc.) Changing `.htacess` with `.DS_Store` got the full flag.

# Some Assembly Required
**Flag :** picoCTF{a8bae10f4d9544110222c2d639dc6de6}<br/>
Simple!
On loading website makes a GET request to get the correct flag. I this junk last line is clearly written flag itself xD.


# where are the robots
Simple!
**Flag :** picoCTF{ca1cu1at1ng_Mach1n3s_477ce}
Clearly, Creator control acces using **robots.txt**. So, get it using GET request and next Hint :

    Disallow: /477ce.html
  get **/477ce.html** and it contains flag.

# logon
Bit error porne!
**Flag** : picoCTF{th3_c0nsp1r4cy_l1v3s_d1c24fef}
As mentioned in Hint login doesn't check password of any other user except Joe. So, first login with any random username and password. On login, it makes request to **/flag** endpoint. Change that request's cookies values. Set 

    username = Joe
    admin = True
**NOTE** : requests are case sensitive.

# dont-use-client-side
Simple!
**Flag :** picoCTF{no_clients_plz_1a3c89}
website doen't make any request to verify cerdentials. So, clearly password is already present in computer and That's it!
Flag is contained in js script which is embedded in html file. It's just broken into parts.

# login
Simple!
**Flag :** picoCTF{53rv3r_53rv3r_53rv3r_53rv3r_53rv3r}
Flag is in encoded form in js file fetched by website to match the password entered. Flag is encoded in base64 format, just decode it!
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5NjExNzE1MDcsLTU0NDg1MzY1LC0xNz
AxNTY5NjgyLC00ODM3MTc2NjYsLTQwNjM3NjE3NywxOTIxNjg3
MDQ3LC00MTU5NDMxMjIsNjE2MTM2ODcxLDE4NzU0NDkxNzAsOT
I1MjA3NzczLDE1NzUxNjk5MjZdfQ==
-->