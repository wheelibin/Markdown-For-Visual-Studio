Markdown Helper For Visual Studio
=================================

About
------

Use the amazing text-to-HTML tool [Markdown](http://daringfireball.net/projects/markdown) to create HTML in Visual Studio.

You can create a markdown file directly in Visual Studio and this tool will output the generated HTML as a file within the project.  

*I am currently using it to output a partial view for ASP.NET MVC3 for a help/FAQ page.*

*It allows me to write the page using Markdown and have the generated file used as a partial view without me having to copy and paste from a markdown converter to Visual Studio.*

How To
------

###Naming Convention for your markdown files

So the tool can infer what file extension you would like to create you should use the following filename pattern:

	filename.[required_extension]_md

examples:

	test1.html_md
	test1.cshtml_md
   
produces:

	test1.html
	test1.cshtml

###Enabling the tool

Set the "CustomTool" property on each of your markdown files to "Markdown".

The HTML output will now be automatically created every time you save the markdown source file.
	
Credits
=======
- A vast majority of the code in this plugin is taken from Steve Potter's excellent [**LessCssForVisualStudio extension**](https://github.com/StevePotter/LessCssForVisualStudio)
- The markdown conversion is done using [**markdownsharp**](http://code.google.com/p/markdownsharp/)
- Obviously the whole reason for doing this is to use Markdown so all credit to [Markdown](http://daringfireball.net/projects/markdown/)