Yet another HTML to PDF Node package, this is just a package i made for myself because i had a problem specifically using HTML to PDF with templates.

This package has two public methods
<h1>test</h1>
* createFromTemplateData(html, htmlData, pdfName, callback)
* createFromHtml(html, pdfName, callback)

Send in string HTML and PDF name!
Usage:
Creating from HTML: node src/main test.pdf <html><h1>test</h1></html>
Creating from HTML template: node src/main test.pdf "<html><h1>{{test}}</h1></html>" "{"test":123}"

The gist of this project is that it should encapsulate the functionality needed to create PDFs from HTML templates, or just pdf from HTML file/html string

I use Handlebars and Phantom-node to achieve this effect.

There should be support for win32/osx/nix
