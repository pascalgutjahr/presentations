# LS8 Poster Template

A tidy poster template with round-edge boxes laid out in three columns.


## Corporate Identity

One of two color palettes must be chosen with the `colorpalette{arg}` macro, where the argument is either `tu` or `ml2r` (see line 39 `poster-template.tex`). Also, you may have to change the header logo and the acknowledgment in the footer of the poster.


## Building

I recommend using `make` to build the poster. This will not only handle the LaTeX build process,
but also generate a well-printable version which is handled correctly by many printer firmwares.

Complete poster: https://bitbucket.org/ls8-tudo/poster-template/downloads/poster-template.pdf


## Road Ahead

The template is to be matured into a nice LaTeX class which separates the layout from the content.
Please let us know if you have additional feature requests. You can also set up a branch directly,
to prepare the features you strive for.

Contact: `mirko.bunse@cs.tu-dortmund.de`
