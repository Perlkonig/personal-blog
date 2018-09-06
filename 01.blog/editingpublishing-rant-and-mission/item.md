---
# http://learn.getgrav.org/content/headers
title: 'Editing/Publishing Rant and Mission'
slug: editingpublishing-rant-and-mission
# menu: Editing/Publishing Rant and Mission
date: 15-06-2012
published: true
publish_date: 15-06-2012
# unpublish_date: 15-06-2012
# template: false
# theme: false
visible: true
summary:
    enabled: true
    format: short
    size: 128
taxonomy:
    category: ["Rants & Ponderings"]
    tag: [editing,writing,XML]
author: aaron
metadata:
    author: aaron

---

Just to clarify, this rant is intended for people interested in professional document production.

My new life’s mission is to convince the publishing world to move to a plain-text-based, XML workflow. Here’s the dirty little secret: [InDesign ](http://www.adobe.com/products/indesign.html)(and even, \*sighs\*, [QuarkXpress](http://www.quark.com/)) is no harder to learn than [Word](http://office.microsoft.com/en-us/word/). In many ways it’s far easier. The problem is that Word *seems* at first glance to be powerful enough for real publishing needs, but as soon as you actually sit down and try to compose anything longer or more complex than a letter to mom, it sinks in how limited it is. I understand that part of the problem is that many people just don’t care how their documents look or even know what looks good. That’s fine, but they’re not my target audience. I want to reach misguided publishers that insist that documents be presented, print-ready, in Word and authors that just don’t yet realize how liberating a plain-text-based workflow is. What the publishing world is missing is an open-source, platform-independent plain-text editor that supports “track changes” capability and straightforward XML markup. I guess it’s up to me to write it! 🙂

From a semantic point of view, very few books need more markup tags than are provided in basic HTML. You just need a few levels of headers, some basic table markup, list tags, and some emphasis tags for kicks. That’s it! You shouldn’t have to worry about depth of margins, how far the lists indent, how exactly the block quotes will appear until *after* the text is finalized.  You certainly don’t need to worry about the exact font face, size, and leading! This is all editors proper should have to work with. Here’s the text, focus directly on content and structure, and ignore everything else. A designer (who could also be the editor) then takes that text and drops it into *proper* typesetting software. By “proper” I mean that it understands what a baseline grid is and why it is important. It can manage a book length project split across multiple files without trouble. It can justify text intelligently. It gives you complete control over kerning. It works with complex fonts and understands things like ligatures and optical margins with little intervention from the user. It can make tables look consistent with relative ease. The list goes on and on. Word can’t do any of this. People think it can. It looks like it should. And sure, “gurus” can make Word mimic real functionality. But fundamentally, it never seems to work exactly as you think it should. Modern publishing workflows (especially when it comes to self-publishing) have increasingly blurred the distinctions between content creation, editing, and design. While this isn’t all bad, I think it does impede the smooth production of high-quality, error-free, well-designed text.

For example, when I worked on [my master’s thesis](http://dspace.ucalgary.ca/handle/1880/47815), I wrote the entire thing using a plain text editor (including all the music). Not only did it make it possible to write anywhere, from any computer, using Notepad (if I really hated myself), it  freed me to focus solely on the text. There was no tweaking of the margins, trying different type faces, fretting about whether or not the B-head should be indented, etc. I cannot express what a liberating experience it was! It also let me work across multiple files if I wanted. The best, best part was the ability to use proper [version control software](http://en.wikipedia.org/wiki/Version_control) (I chose [Subversion](http://subversion.apache.org/)). Authors around the world, I beseech you to learn how version control can change your life! What was the major hurdle I faced? Track changes. Because there is no plain-text editor I’ve yet found that supports the track changes features of Word, I had to jump through some hoops to make my text easily accessible to my advisor for editing. Once we were happy with the text, then what? Well if I were to do it all over again, I’d do it in InDesign. Because I’m somewhat of a masochist, and I had been using this software throughout my university career, I used [LaTeX](http://www.latex-project.org/) combined with [BibTeX](http://www.bibtex.org/) and [Lilypond](http://lilypond.org/). *This* was when I fretted about margins, indentation, figure placement, line breaks, and all that design stuff.

Now in this example I didn’t actually use HTML/XML markup in my text, but that’s how I think it should be. This offers a huge benefit to the document production side of things. Once you have semantically marked-up text that is as perfect as it can be, it can now be transformed into many different formats. Want a web page? If marked-up properly, it’s trivial to add the text to a website. Want an ePub? Also trivial. Want to import into InDesign? InDesign (because it’s awesome) will let you associate tags with specific style sheets. A few mouse clicks and your book is 90% set! All of this can be derived from a single master file, which can be easily stored in a format that will never become obsolete: plain text.

I could go on, but 900 words is enough. In short:

1. Content creators shouldn’t have to worry about or be distracted by design issues. Focus on the content.
2. Microsoft Word should be replaced by a plain-text editor that encourages semantic markup and includes track-changes functionality.
3. The resulting XML document can then be transformed into any number of formats at the design stage.
4. Clearly distinguishing between these different phases of production, combined with using the right tool for the job (and Word is never the right tool for any job), will greatly facilitate the production of high-quality, error-free, well-designed text.

