# Bandit Level 10 to 11 Writeup

Author: [Naman Singla](https://github.com/nsingla20)

Problem Page: [bandit10](https://overthewire.org/wargames/bandit/bandit11.html)

## List of Commands Used
```
sshpass - For Authentucating ssh with scripts
ssh	- To login to remote server using user id
clear	- to clear the current screen for cleaner output
base64	- For decoding the given text
exit	- To close the connection to ssh server
```

## Walkthrough
Just came to know about command base64 given in list on website. Then googled it to check its use.

## Password
`IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR`

## Bash/Python script to automate the process
```
#!/bin/bash
sshpass -p "truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk" ssh -tt -o StrictHostKeyChecking=no bandit10@bandit.labs.overthewire.org -p 2220 <<HERE
clear
base64 -d data.txt
exit
HERE
```

## Suggested modifications [Optional]
What can you do to make this level more difficult. The inherent idea should be similar.
