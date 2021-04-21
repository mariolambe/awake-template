---
title: How to Extract URLs from Webpages
subtitle: SEO
category:
  - About Awake
author: Mario Lambertucci
date: 2021-03-01T18:35:46.114Z
featureImage: /uploads/markup-hero.jpg
---
If you are wondering **how to extract URLs from any webpage**, for free, really fast you are in the right place!

I selected the best 3 methods:

* Browser
* Addon
* Terminal

Let’s jump right into it.

## **1. Extract URLs from webpages with your browser:**

You will need:

* a browser
* piece of code 

![Extract URLs from Webpages](https://user-images.githubusercontent.com/61537859/114431238-8f4a4480-9bbf-11eb-9eaf-7b5cf7d2cb0e.gif)

Navigate to the page from which you’d like to extract links.

Right-click the page and select “Inspect”. 

This will open up the console, into which you can type or copy and paste this code:

```
var x = document.querySelectorAll("a");
var myarray = []
for (var i=0; i<x.length; i++){
var nametext = x[i].textContent;
var cleantext = nametext.replace(/\s+/g, ' ').trim();
var cleanlink = x[i].href;
myarray.push([cleantext,cleanlink]);
};
function make_table() {
    var table = '<table><thead><th>Name</th><th>Links</th></thead><tbody>';
   for (var i=0; i<myarray.length; i++) {
            table += '<tr><td>'+ myarray[i][0] + '</td><td>'+myarray[i][1]+'</td></tr>';
    };
 
    var w = window.open("");
w.document.write(table); 
}
make_table()
```

## **2. Extract URLs from webpages with addons:**

I can reccomend a really powerful Chrome addon called [Link Klipper](https://chrome.google.com/webstore/detail/link-klipper-extract-all/fahollcgofmpnehocdgofnhkkchiekoo?hl=en)

![Link-Klipper](https://user-images.githubusercontent.com/61537859/114427036-f9acb600-9bba-11eb-9c39-badb724132b5.jpeg)

This extension allows you to :

* Extract all the links on the webpage
* Store all the extracted links as a CSV file
* Custom drag a selectable area on the webpage from which all the links will be extracted

## **3. Extract URLs from webpages with the terminal:**

That´s what you´ll need to do the magic:

* MAC
* termnial
* wget installed

First of all check if you already installed wget by running the following command:

```
$ wget -V
```

If it is not installed yet then install 
[Homebrew](https://brew.sh/) first:

```
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Then you need to install wget:

```
$ brew install wget
```

Now you got everything you need to **extract URLs from a webpage** for free with only one single command:

```
$ wget --mirror --delete-after --no-directories https://www.the-page-you-wanna-crawl.com 2>&1 | grep '^--' | awk '{print $3}' | sort >extracted-URLs.txt
```

The command will export all the URLs in a txt file called extracted-URLs.txt (if you want you can also rename it).

This method was shared via Twitter by John Muller.

Have fun!