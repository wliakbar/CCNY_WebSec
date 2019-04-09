# Project 7 - WordPress Pentesting

Time spent: **X** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) Vulnerability Name or ID: WordPress <= 4.2.2 - Authenticated Stored Cross-Site Scripting (XSS)
  - [ ] Summary: This challenge basically exploited a cross site scripting vulnerability in which if the user simply has to mouse over the link.
    - Vulnerability types: Stored Cross-Site Scripting (XSS)
    - Tested in version: 4.2.2
    - Fixed in version: 4.2.3
  - [ ] GIF Walkthrough:![Lab8_Chal1](https://user-images.githubusercontent.com/32075350/55765807-6bd3e880-5a3f-11e9-8e84-a90d9581913b.gif)
  - [ ] Steps to recreate: To recreate this vulnerability simply create a post with the following text: <a href="[caption code=">]</a><a title=" onmouseover=alert('HACK') ">link</a>
  - [ ] Affected source code: post.php
    - [Link 1](https://core.trac.wordpress.org/browser/tags/4.2.2/src/wp-admin/post.php)
1. (Required) Vulnerability Name or ID: WordPress  4.0-4.7.2 - Authenticated Stored Cross-Site Scripting (XSS) in YouTube URL Embeds
  - [ ] Summary: This explot take advantage of a XSS vulnerabilty where youtube link embedded into a post triggers the exploit.
    - Vulnerability types:Stored Cross-Site Scripting (XSS)
    - Tested in version:4.2.2
    - Fixed in version: 4.7.3
  - [ ] GIF Walkthrough: ![Lab8_Chal2](https://user-images.githubusercontent.com/32075350/55766014-9a05f800-5a40-11e9-980e-ceba61acdfc6.gif)
  - [ ] Steps to recreate: Simply type the following text into a post: [embed src='https://youtube.com/embed/12345\x3csvg onload=alert(1)\x3e'][/embed]
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code: media.php
    - [Link 1](https://core.trac.wordpress.org/browser/tags/4.2.2/src/wp-includes/media.php)
1. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
