
## Web Explorer
<p float="left">
  <img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" />
  <img src="https://img.shields.io/badge/-playwright-%232EAD33?style=for-the-badge&logo=playwright&logoColor=white" />
</p>

![img](https://raw.githubusercontent.com/kishism/web-explorer/refs/heads/main/Screenshot1.png)
Simple text-based browser like classic **lynx** and **w3m**, with simple navigation.
It is powered by ***Playwright*** under the hood.

 Web Explorer is a lightweight, text-based web browser that is built on top of playwright, and make with Python. Inspired by classic terminal browsers like w3m, and lynx, it allows users to navigate websites, follow links (primarily), and explore content without leaving the terminal.

Of course, the major (and it's most obvious) limitation of such browser is that it is not guaranteed to display SPA (Single Page Application) pages without employing some sort of custom script to do that. Crawling such sites typically results in empty content, as the browser only extracts the static HTML skeleton.

I called this a crawler because, technically speaking, Playwright crawls the targeted site, and extract the HTML skeleton, and the code simply parses, and maps each node. It then represents the content with Rich text in a readable format.. (for example `<h1>` tags become "Heading,", `<p>` tags becomes paragraphs, etc ) without changing the original hierarchical structure of the page. 
