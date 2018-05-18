# week-7
# Project 7 - WordPress Pentesting

Time spent: **20** hours spent in total

> Objective: Find, analyze, recreate, and document **three vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. Unauthenticated StorCrossed -Site Scripting (XSS)
  - [ ] Summary: 
    - Vulnerability types: 
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [ ] GIF Walkthrough: ![1 4](https://user-images.githubusercontent.com/37822922/40213482-875005f2-5a0a-11e8-92ad-09aa70a5a6b0.gif)
  - [ ] Steps to recreate: You would need to type in a code with over 64kb of comments in order for it to work. Such as the following: <a title='x onmouseover=alert(unescape(/hello%20world/.source)) style=position:absolute;left:0;top:0;width:5000px;height:5000px  AAAAAAAAAAAA...[64 kb]..AAA'></a> once this is done you would press submit and an alert box pops up.
  - [ ] Affected source code:
  
2. Fingerprinting 
The WordPress 'http://wpdistillery.vm/readme.html' file exists exposing a version number
  - [ ] Summary: One is able to see the version number which is not updated to the current 4.9. Therefor one can find the vulnerabilities available with that version of WordPress and attack it in that manner. 
    - Vulnerability types:
    - Tested in version: 4.2
    - Fixed in version: 
  - [ ] GIF Walkthrough:![2 3](https://user-images.githubusercontent.com/37822922/40213483-885f20c2-5a0a-11e8-8d77-71d164ce6270.gif)
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
  
3. Privilege Escalation
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough:![3 2](https://user-images.githubusercontent.com/37822922/40214119-e56e3e9e-5a0d-11e8-8efc-1a1a3e66bd85.gif)
  - [ ] Steps to recreate: 
  - [ ] Affected source code:<img width="1312" alt="screen shot 2018-05-17 at 8 12 12 pm" src="https://user-images.githubusercontent.com/37822922/40214271-a99e37ec-5a0e-11e8-8508-1e00fcb6d1bb.png">
