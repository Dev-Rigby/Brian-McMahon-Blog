---
template: blog-post
title: Google Lighthouse, A Guide to a Better Site
slug: /lighthouse
date: 2021-01-31 22:31
description: Article about Google Lighthouse
featuredImage: /assets/lighthouse640x452.png
---
<!--StartFragment-->

For web developers the one of the most important tasks is care and feeding of their websites. This includes making sure that all modules are up to date and making sure that your code uses the current best practices. When running multiple sites this can become a big chore that one could get lost in. For those people google has released a service called Lighthouse. Lighthouse can be run against any web page, public or private. It runs tests on the performance, accessibility, vulnerabilities, and more. The program can be run in devtools, command line, or as a node module. Being open source the program can also be edited to test for more than what is included currently.

I ran Lighthouse on my website from Web Dev I to see how it would do and here are the results:

![](https://lh6.googleusercontent.com/RjLqzNmyWl_0sgNH1QKgFalAPPL7gyEiO0cJj_D3_ymo4cImwcxcuSOe6vOp9byGxFQDKq2Le8MXXtyvRhVcD4hjg9suSCTvpY-8vqRuLnlleR3ABjTTWZaJ_o3kFD63Jn9lb2C7)

My website got a 99 in performance, 93 in accessibility, 86 in structure and 92 in SEO. Lighthouse allows you to look through these sections for tips on how to improve the score of the site. These metrics allow site owners the ability to audit their site in an unbiased way. Sometimes developers are asked to come and improve a website and a tool like this is very powerful for finding a starting point. One thing that I was unable to do was change the device that Lighthouse ran the test on. The program preselected the Moto G4 and ran the test on the site at that responsive state. I am not sure how this affects the scoring. The program shows all the information surrounding an issue so that a decision on what to do can be made. Here is a closer look under the best practices section:

![](https://lh5.googleusercontent.com/z_kEmEeVAEMNnteuApk69_HFgKvMPsZINPGwMxwX5HmpeSDaIXKlf0rdYHEaMJX7to4qBx-ysRjmXyqHz4XK5Qe0CBEMdg4R7xO55ilHqBJp3ajJQRkDnTpRI__dsudyrGrLWooA)

These reports can also be shared and reviewed online. Lighthouse allows for the report to be exported as a json file or as a github gist. Through doing research I was able to find two other solutions that rival Lighthouse, SpeedCurve, and GTmetrix. I decided to test out GTmetrix to see how it compares to Lighthouse. So I ran GTmetrix on my about me website like I did with Lighthouse and here were the results:![](https://lh4.googleusercontent.com/WHjNYXNgn5qlv0zWjcWAYWAXiP_bOSLsqU2jD2d6Xla-0WPzQHninAO9o31s-P_nQBHQ9o9hHzk2bSFeCF8EJjCrsjB2kN_rvMkz-ojpVIyCMCTE92u0eBH9amfk5Qm6-G7jieBT)

My score in GTmetrix was almost the same as Lighthouse and they both focused on the same images when scoring my page. The fact that the scores were so similar made me disregard the fact that Lighthouse ran the test on the Moto G4 responsive state. This shows that either one of these solutions provide good metrics for auditing personal or professional websites. Tools like these not only help to improve websites but also teach better practices for those who create them. As websites are improved with these programs so are the future websites of the user.



Objectives

* Explain Lighthouse
* Show and Talk About Results
* Show and Talk about comparison to competitor

Resources

* <https://developers.google.com/web/tools/lighthouse/#devtools>
* <https://www.reddit.com/r/webdev/comments/hmnt08/do_you_use_google_chrome_lighthouse_to_measure/>
* <https://gtmetrix.com/>

<!--EndFragment-->