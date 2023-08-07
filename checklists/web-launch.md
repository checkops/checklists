---
title: Website Launch Checklist
category: Front-End
date: "2023-08-01"
tags: ['launch', 'website']
description: Checklist for all things you need before you launch your website or webpage.
featured: true
---


### PERFORMANCE

- [ ] Web Page Size should be under 1MB  
The webpage size consists of all the files that make up a page. A typical web page is made up of several files that may include HTML, CSS, Javascript, or image files, as well as other resources.Keep this below 1MB so that its quicker to download.

- [ ] Minify your Web Page  
Minify your HTML,CSS and JavaScript files to reduce page weight. Minification works by removing or transforming the content of these files in a way that preserves the behaviour of the code but reduces the file size.Read More below <br>[google minification guide](https://developers.google.com/speed/pagespeed/insights/)<br>

- [ ] Compress your WebPage Resources  
Configure your server to send data in a compressed format to reduce transfer times.Text-based data formats such as HTML, CSS, JavaScript, plain text, XML, JSON and SVG should almost always be sent with compression enabled.Read More below <br>[google compression guide](https://web.dev/optimizing-content-efficiency-optimize-encoding-and-transfer/)<br>[mozilla compression guide](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Encoding)<br>

- [ ] Check for Cookie Size Limits  
If you are using cookies be sure each cookie doesn't exceed 4096 bytes and your domain name doesn't have more than 20 cookies.Read More below <br>[Cookie specification: RFC 6265 ](https://datatracker.ietf.org/doc/html/rfc6265)

- [ ] Minimize Third Party domains and components  
Third party iframes or components relying on external JS.For each of different domains , the browser needs to make a DNS look-up, which is slow. Avoid having to many different domains and the page should render faster.

- [ ] Enable Caching with long caching times   
Enable caching of your page resources so browsers can reuse resources that have already been downloaded.Configure page resources to have long caching times so browser caches will retain them for longer. Read More below <br>[HTTP Caching Guide by Google ](https://web.dev/http-cache/)

- [ ] Avoid Inline and Blocking JavaScript   
Ensure You don't have any JavaScript code inline (mixed with your HTML code).JavaScript files should be loaded asynchronously using async or deferred using defer attribute. Read More below <br>[Non Blocking JS Guide by Google ](https://developers.google.com/speed/docs/insights/BlockingJS/)

### SEO

- [ ] Set proper page titles  
Every page should be given a title that describes its content. Well-written titles are vital for improving the search rank of pages because search engines look for keywords in titles to determine how relevant pages are to search queries.<br>[google page title guide](https://support.google.com/webmasters/answer/35624?hl=en)<br>

- [ ] Set proper meta description  
Every page should be given a title that describes its content. Well-written titles are vital for improving the search rank of pages because search engines look for keywords in titles to determine how relevant pages are to search queries.<br>[google page title guide](https://support.google.com/webmasters/answer/35624?hl=en)<br>


- [ ] Set proper page headings   
A meta description is provided, it is unique and doesn't possess more than 150 characters.Read More below <br>[Meta Description - HTML - MDN](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#adding_an_author_and_description)<br>

- [ ] Robot.txt is present and updated  
Add a robots.txt file to every subdomain so you can specify sitemap locations and set web crawler rules. Robots.txt files are always located in the root folder with the name robots.txt.Read More below <br>[Robot.txt guide by google](https://developers.google.com/search/docs/crawling-indexing/robots/intro)

- [ ] Setup Sitemap page and Keep it updated  
An HTML sitemap is provided and is accessible via a link in the footer of your website.Sitemap files contain a list of page URLs that you want indexed and are read by search bots. These files can also include metadata that describes when pages were last updated.Read More below <br>[Sitemap guide by google](https://developers.google.com/search/docs/crawling-indexing/sitemaps/build-sitemap?hl=en&visit_id=638264877284613311-2158601090&rd=1)

- [ ] Check and Avoid Broken Links   
All internal and external  links on your website should be valid and working.Broken links can signal to search engines that your site is poor quality and will frustrate users. 


- [ ] Handle Error Pages for Broken Urls     
Ensure Error pages are created for standard errors like 404,500 errors . Read More below <br>[Error Page Guide by Google ](https://developers.google.com/search/docs/crawling-indexing/http-network-errors?hl=en&visit_id=638264878507918336-198191165&rd=1#soft-404-errors)

- [ ] Check for social meta tags for shared links preview       
Facebook OG and Twitter Cards are, for any website, highly recommended but you can check more depending on social media where you want to share.You Can Check more below <br>[Facebook OG testing](https://developers.facebook.com/tools/debug/)<br>[Twitter card validator
](https://cards-dev.twitter.com/validator)

### SECURITY

- [ ] Always use HTTPS     
HTTPS is used on every page and for all external content (links,plugins, images,etc..). Read More below <br>[Why HTTPS by Google](https://web.dev/why-https-matters/)

- [ ] Check HSTS is enabled  
Configure HSTS (HTTP Strict Transport Security) response headers to force browsers to always use HTTPS instead of HTTP on your site.. Read More below <br>[HSTS Check](https://hstspreload.org/)

- [ ] Check updated TLS in use    
Check weather your page or website is on latest TLS 1.3 as TLS 1.1 and 1.2 are deprecated. <br>[Why OLD TLS is unsecured?](https://www.appviewx.com/blogs/why-is-tls-1-3-better-and-safer-than-tls-1-2/)


- [ ] Check X-Frame-Options (XFO) header is Enabled   
Check X-Frame-Options (XFO) header is Enabled which protects your visitors against clickjacking attacks. <br>[Clickjacking by OWASP](hhttps://owasp.org/www-project-web-security-testing-guide/v41/4-Web_Application_Security_Testing/11-Client_Side_Testing/09-Testing_for_Clickjacking)

- [ ] Check Content Security Policy is Enabled   
Defines how content is loaded on your site and from where it is permitted to be loaded. Can also be used to protect against clickjacking attacks. <br>[CSP Check](https://content-security-policy.com/)

- [ ] Check XSS protection is Enabled    
Check weather your page or website is free from XSS possible issues to avoid malicious code injections. <br>[XSS Check](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-XSS-Protection)


### DESIGN

- [ ] Check for Responsive Web Design    
The website is using responsive web design. All pages were tested at the following breakpoints: 320px, 768px, 1024px (can be more / different according to your analytics).Check  below <br>[Responsive Test](https://responsivedesignchecker.com/)

- [ ] Check On Different Browsers   
All pages were tested on all current desktop browsers (Chrome , Firefox, Safari, EDGE...) as well as mobile browsers (Native browser, Chrome, Safari...).

- [ ] Check for Webfont format   
WOFF, WOFF2 and TTF are supported by all modern browsers. Ensure Webfont sizes don't exceed 2 MB. Check  below <br>[WOFF Compatibility](https://caniuse.com/woff/) 


- [ ] Check for Favicons Setup    
Favicon has been created and displays correctly. PNG format is recommended over .ico format (dimensions: 32x32px). Check  below <br>[Favicon Compatibility](https://caniuse.com/link-icon-png) 




### ACCESSIBILITY

- [ ] Check for Proper Headings    
Headings should be used properly and in the right order (H1 to H6). There should be only 1 H1 per page

- [ ] Check for Form Labels   
A label is associated with each input form element. In case a label can't be displayed, use aria-label instead.<br>[Using Labels](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-label/)

- [ ] Check for Image Setups   
Provide layout images 2x or 3x, support retina display.Set width and height attributes on <img> if the final rendered image size is known. Also All <img> have an alternative text which describes the image visually.

- [ ] Check for Color contrast   
Color contrast should at least pass WCAG AA (AAA for mobile).<br>[Contrast Check](https://color.a11y.com/)

- [ ] Check for Keyboard navigation    
Test your website using only your keyboard in a previsible order. All interactive elements are reachable and usable. 