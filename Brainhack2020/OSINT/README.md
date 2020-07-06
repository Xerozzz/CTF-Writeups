# OSINT

## Better Alternative Than TV
### Challenge
Looks like we found a clue to the mastermind behind the brainwashing liquid.

The company's name is UnduplicitousCorp, sounds kinda fishy. Let's conduct some basic reconnaisance and see if there's any videos about the company on social media.

### Solution

Paste "UnduplicitousCorp" into google search bar. Look for the channel named "UnDuplicitousCorp Tech". The flag is located in the About section of the channel.

### Flag

CDDC20{S+@rt_O$!nT}

## Fun with File Extensions

### Challenge

Now that we have their company website, it will be helpful for us to know how the company layout is like.

### Solution

In the About section of the youtube channel, there is a link to the company's website: [here](https://www.unduplicitouscorp.tech/index.html)
In the About page of the website, there is a link which brings you to an organisational chart of their company: [here](https://www.unduplicitouscorp.tech/Organisation%20Chart.pdf)
There appears to be some text resembling a flag hidden beneath the diagrams of the chart. There is also a hint at the bottom right "I wonder how to get an editable version of this". To get an editable version, we can convert the pdf to a word document.
The final step is simply to move away the diagram which is covering the flag.

### Flag
CDDC20{EV!L_CORP_CH@RT}

## OSINT-3 Transparency is the Best Policy
### Challenge
The website looks state-of-the-art. As expected of a evil mega conglomerate.

Okay, they're using HTTPS certificate, very secure. Is there any way we can discover what other domains they are hosting?

### Solution
Previously we got the link "https://www.unduplicitouscorp.tech/index.html". Hint is HTTPS certs, so if we go to crt.sh and input the domain "unduplicitouscorp.tech", we can see that there are other domains that is being hosted too. IN particular, we want to go to "flag.tt7ncdhj367dh8mu2pb6.unduplicitouscorp.tech" Our flag is right there

### Flag
CDDC20{CERT_TR4SP4RENCY}

## Funky Transmission

### Challenge

Being such a huge conglomerate, it can't be that they only have a tiny web server..

### Solution

The name of this challenge is "Funky Transmission", wonder what that means? Maybe can try ftp into [the server](https://www.unduplicitouscorp.tech)...
Entered [ftp://www.unduplicitouscorp.tech/](ftp://www.unduplicitouscorp.tech/) into the browser, am granted anonymous access. Flag is located in "flag.txt" file.

### Flag

CDDC20{@n0nymous_FTW}

## Follow the Breadcrumbs

### Challenge

Following the breadcrumbs, this employee seems like an aspiring photographer.

### Solution

There are 3 pptx files in the ftp server, I download all of them, there is a flickr profile link in the second pptx file. Seems that this is the photography account of the mentioned employee.
Upon clicking on the "Album" section, there is an album named "Projects"...the flag is located in the page header for this album.

### Flag

CDDC20{Fl!ckr_0h_Flick3r}
