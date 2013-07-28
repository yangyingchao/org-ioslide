## ox-ioslide.el
*Export org-mode to Google I/O HTML5 slide..*

---

### Note: This emacs plugin is under hardly development.


It's not suggest to use this plugin since
any function may be renamed or modified later.


ox-ioslide.el works like org-html5presentation.el and generate
Google I/O 2013 slide template.


### Installation (not done yet)


If you have `melpa` and `emacs24` installed, simply type:

     M-x package-install org-ioslide

In your .emacs

     (require 'ox-ioslide)

### Function Documentation


#### `(org-ioslide-get-hlevel INFO)`

Get HLevel value safely.
If option "HTML5SLIDE_HLEVEL" is set, retrieve integer value from it,
else get value from custom variable `org-ioslide-hlevel`.

#### `(org-ioslide-center-block CENTER-BLOCK CONTENTS INFO)`

Transcode a CENTER-BLOCK element from Org to HTML.
CONTENTS holds the contents of the block.  INFO is a plist
holding contextual information.

#### `(org-ioslide-stylesheets INFO)`

Return the HTML contents for declaring ioslide stylesheets.

#### `(org-ioslide-export-block EXPORT-BLOCK CONTENTS INFO)`

Transocde a EXPORT-BLOCK element from Org to ioslide.
CONTENTS is nil. NFO is a plist holding contextual information.

#### `(org-ioslide-src-block SRC-BLOCK CONTENTS INFO)`

Transcode a SRC-BLOCK element from Org to HTML.
If #+USE_PRETTIFY is `true` use org-ioslide--src-block to render the code block.
Else use org-html-src-block to convert source block to html.

#### `(org-ioslide-headline HEADLINE CONTENTS INFO)`

Transcode a HEADLINE element from Org to html5presentation.
CONTENTS holds the contents of the headline. INFO is a plist
holding contextual information.

#### `(org-ioslide-section SECTION CONTENTS INFO)`

Transcode a SECTION element from Org to HTML.
CONTENTS holds the contents of the section. INFO is a plist
holding contextual information.

#### `(org-ioslide-template CONTENTS INFO)`

Return complete document string after HTML conversion.
contents is the transoded contents string.
info is a plist holding eport options.

#### `(org-ioslide-download-resource)`

Download extra resource like css or js file to use this slide offline.

<!-- Error: (void-function &optional) -->

<!-- Error: (void-function &optional) -->

-----
<div style="padding-top:15px;color: #d0d0d0;">
Markdown README file generated by
<a href="https://github.com/mgalgs/make-readme-markdown">make-readme-markdown.el</a>
</div>
