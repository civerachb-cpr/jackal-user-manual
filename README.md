Jackal User Manual
==================

To build Jackal's user manual, run:

    git clone --recursive https://github.com/jackal/jackal-user-manual.git
    xelatex jackal.tex

The output is written to `jackal.pdf`. The `xelatex` command must be invoked twice
to generate the complete manual including table of contents and correct watermarks.


Setting it up
-------------

The manual may be built on any platform supported by TeXWorks or TeXLive.

On a **Mac**, download and install [MacTex Basic](http://mirror.ctan.org/systems/mac/mactex/mactex-basic.pkg).

On **Ubuntu**, run:

    sudo apt-get install texlive-xetex

Install some additional texlive packages:

    sudo tlmgr install everypage background titlesec microtype upquote \
                       enumitem tcolorbox environ trimspaces siunitx

On **Windows**:
- Install TeXworks
- Install DINPro font (from our server) into your system fonts
- Install Source Tree and register accounts. Remeber BitBucket uses full email address.
- Checkout a LaTeX document, and open it in TeXworks
- In Texworks, in the drop down menu beside the green arrow, switch to XeLaTeX + MakeIndex + BibTex
- Click the green start arrow


Typefaces
---------
To build the official manual, the following fonts will need to be installed:

- DINPro
- [Consolas](http://www.fontpalace.com/font-download/Consolas/)


Visuals
-------

The visual components including diagrams and cover page are SVG documents created using Inkscape. [Download
this for your platform](http://www.inkscape.org/en/download/) to edit these components. When you are ready
to integrate the edited component into the manual, you must export it to a PDF in the `gen` folder.

For the cover page:
* Full page output, including text.

For diagrams and illustrations:
* Exclude text, also render LaTeX.


License
-------

Redistribution and use in source and binary forms, with or without modification, is
not permitted without the express permission of Clearpath Robotics.
