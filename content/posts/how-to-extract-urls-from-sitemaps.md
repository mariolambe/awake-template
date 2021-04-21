---
title: How to Extract URLs from Sitemaps
subtitle: SEO
category:
  - About Awake
author: Mario Lambertucci
date: 2021-04-01T18:35:46.114Z
featureImage: /uploads/markup-hero.jpg
---
If you are wondering how to extract sitemap URLs really fast you are in the right place!

There are different options out there and I selected the best 3 methods:

- Google Sheets
- Screaming Frog
- Terminal
 

Let’s jump right into it.


## **1) Extract URLs From XML Sitemaps Online In Google Sheets**

I found a simple sitemap extractor script that will extract the list of URLs from the Sitemap in Google Sheets in less than 5 seconds, pretty impressive, isn’t it? Give it a try.

[Here the Google Sheet that act as a sitemap url extractor:](https://docs.google.com/spreadsheets/d/1U549m-mcSHIwebpMzjDr3s5ggO95LAnf7YbccrwUkoE/copy)


1. Make a copy of it

2. Add the sitemap URL in the cell B2 (example: https://www.google.com/sheets/sitemaps.xml)

3. The list of URLs will appear automatically in column D

4. Done! You have just converted your sitemap to a URL list.

![import_sitemap_urls_google_sheets](https://user-images.githubusercontent.com/61537859/111198585-0213d000-85c0-11eb-9fe1-f674f5db8e86.jpg)



## **2) Extract URLs From XML Sitemaps with Screaming Frog**

For this second method you need to install the SEO software Screaming Frog to convert any sitemap xml to a url list. This method works pretty well also for sitemap index file that are the ones that contain list of sub-sitemaps.

Here the steps:

1. Open Screaming Frog SEO Spider Tool

2. Mode>Select List

3. Upload>Download Sitemap>Add Sitemap xml URL

4. Done!

![Import_sitemap_urls_screaming_frog](https://user-images.githubusercontent.com/61537859/111198474-e14b7a80-85bf-11eb-8ea3-3cce18dea492.jpg)



## **3) Extract URLs From XML Sitemaps with command line tools**
1. Open your terminal

2. Enter this command (remember to replace the sitemap URL)-> curl -s https://www.google.com/sheets/sitemaps.xml

3. Done!

![Extract URLs from sitemap](https://user-images.githubusercontent.com/61537859/111198366-c37e1580-85bf-11eb-8484-2d4c5ec3816c.gif)


I hope you find it useful.


