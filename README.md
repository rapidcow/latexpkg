# latex packages i wrote for myself

WARNING: extremely amateur code ahead!!1!!!111


## how to install

taking hmk.dtx as an example...

run this (this creates everything you'll need)

    make

or more specifically:

    make hmk.sty

then copy the generated `hmk.sty` file into your `texmf-local/` directory
somewhere

*   on my MacBook if i run `kpsewhich` on some random class/package
    this happens:

        $ kpsewhich article.cls
        /usr/local/texlive/2021/texmf-dist/tex/latex/base/article.cls

    so place it in `/usr/local/texlive/texmf-local/tex/local/hmk.sty`
    (you might have to create some directories...)

and for documentation (run this 2+ times cuz uh cross-referencing):

    make hmk.pdf

yay (now you should be able to see `hmk.pdf`)

put all this stuff in the same place (`/usr/local/texlive/texmf-local`)
except this time put it in `doc/local` instead of `tex/local` :D

after you're done you probably should run

    texhash


## documentation

this should work

    texdoc hmk


## usage

    \usepackage{hmk}
