# Trip To Us

## Description

IIT kharakpur is organizing a US Industrial Visit. The cost of the registration is $1000. But as always there is an opportunity for intelligent minds. Find the hidden login and Get the flag to get yourself a free US trip ticket.

## Solution:

1. **Finding the 'Click Here' Button**:
    Locate a website featuring a button labeled 'Click Here'. Upon clicking it, I was redirected to `/Error.php`. However, upon inspecting a hidden div, I discovered instructions instructing me to change the User Agent to 'IITIAN'.

![Home Page](../images/home_page.png)
![Error Page](../images/Error_page.png)
![Hidden Div](../images/hidden_div.png)

2. **Changing the User Agent**:
    After changing the User Agent to 'IITIAN', I was redirected to another page containing a login form.

![Home Page](../images/change_user_agent.png)
![Hidden Div](../images/redirect_to_login_page.png)
![Login Page](../images/login_page.png)

3. **Exploiting SQL Injection**:
    Utilizing a SQL injection in the pass parameter, I successfully exploited the vulnerability. Payload used: `'OR id LIKE '1

![Sqli Pyload](../images/sqli_payload.png)
![Flag](../images/web_flag_login.png)

> Flag: VishwaCTF{y0u_g0t_th3_7r1p_t0_u5}
