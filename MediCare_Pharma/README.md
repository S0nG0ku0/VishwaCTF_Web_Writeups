# MediCare Pharma

### Description:
Greetings form MediCare Pharma!!!!

We have started a very new pharmacy where we have various surgical equipments (more to be added soon).

But recently some hackers took control of our server and changed a hell lot of things (probably wiped out everything). Luckily we have few of the accounts and we need more consumers on board. For security reasons, we have disabled SignUp, only authorised persons are allowed to login.

Have a look at our pharmacy and hope we grow again soon.

#### Steps:

- Firstly, I conducted an SQL injection attack on the login page using this payload: 'OR pass LIKE '%. This allowed me to retrieve all users in the database.

- Secondly, I logged in with the user I found earlier, which granted me access to a web page featuring a shopping interface.

- Thirdly, while inspecting the JavaScript script on the web page, I discovered that if I purchase a needle with a quantity greater than 0, the site provides me with a file named upload.php.

- Lastly, I found that by entering any command line into the search tab on upload.php, I could execute it. This led me to discover the flag located in /root/flag.txt.