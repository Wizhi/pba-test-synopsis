# make sure scons finds tex executables:
import os

env = Environment(ENV=os.environ)

env.Replace(BIBTEX='biber')

pdf_output = env.PDF(target='build/main.pdf', source='src/main.tex')

env.AppendUnique(PDFLATEXFLAGS='-shell-escape')

# vi: ft=python
