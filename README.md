Compiled with pandoc and the LaTeX pdf engine.

    pandoc qttutorial.md -o qt.pdf -V colorlinks=true \
    -V linkcolor=blue \
    -V urlcolor=red \
    -V toccolor=gray \
    -V geometry:"left=3cm, top=2cm, right=3cm, bottom=2cm" \
    -V fontsize=12pt

