# Web

## Web-1 No Time
### Challenge
Our project manager couldn't handle the stress from the upcoming deadlines and resigned hastily. Sigh. Now that we are taking over his projects, I wonder if he has left any instructions for us...

http://notime.chall.cddc2020.nshc.sg:1337/

### Solution
Go to the webpage and inspect the element or page source. If you dig a bit you can find a comment with the flag

### Flag
CDDC20{N0_71m3_nO_tiMe_oMG}

## Web-2 VulnLogin
### Challenge
This is not how you log someone in!

http://vulnlogin.chall.cddc2020.nshc.sg:8090/

### Solution
Look under Developers Tool in chrome, in login.js contains :

function login() {
	var username = document.forms[0].username.value;
	username = CryptoJS.MD5(username).toString();
	var password = document.forms[0].password.value;
	password = CryptoJS.MD5(password).toString();
	if (username == "200ceb26807d6bf99fd6f4f0d1ca54d4" && password == "bbb0ddff1b944b3cc68eaaeb7ac20099") {
		alert("CONGRATS! Go ahead and submit your well-earned flag ;)");
	}
	else {
		alert("Login failed! :(");
	}
}

I utilised this website: https://hashes.com/en/decrypt/hash

200ceb26807d6bf99fd6f4f0d1ca54d4:administrator
bbb0ddff1b944b3cc68eaaeb7ac20099:password12345678


### Flag
CDDC20{administrator_password12345678}

## Web-3 Keep Me Posted
### Challenge
Some weird page. Looks fishy. Please help.

http://keepmeposted.chall.cddc2020.nshc.sg:1057/

### Solution
When you go to the page, you see a line of text asking you to "post it a letter". Using an application called Postman, I sent a POST request to the server and got this back:
```You are not authorized :(```

When looking at the Response Headers from the site, the Authorization header looks pretty suspicious. "Tm8=". Looks like base64 encoding. I went to decode it and it gave "No". I went to encode "Yes" into base64 format and sent it as a POST request with an Authorization Header to the website again, this time, it returned the flag :D

### Flag
CDDC20{YEs5SS_1_4m_aUTh0r1z3DDdD}