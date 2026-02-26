# fretboard_quiz_randomizer
A program to create printable PDF worksheets for guitar fretboard memorization practice.

### Project Overview
This project uses PythonTex to automate the creation of randomized fretboard worksheets. Each compile
generates five new randomizations in PDF format. Worksheets display two guitar fretboards, for first-person
and third-person perspective, each with fret spacing given by 12-tone equal temperment tuning.

### Key Features
* Randomized quizzing feature. Each fretboard features blank circles in 16 randomly-selected fretboard
  positions, to promote quick recall of note positions independent of memorized sequences.
* Student and teacher perspective. The upper fretboard represents the teacher's guitar neck, seen from
  third-person perspective. The lower fretboard represents the student's own guitar neck from first-
  person perspective.
* Equal temperment tuining. Frets are placed to scale according to 12-tone equal temperment tuning. This
  accurately models the precise spacing of frets on the guitar fretboard, optimizing the map between the
  worksheet and the real guitar.

### Dependencies
* TeX Live or other LaTeX distribution with the pythontex and TikZ packages
* Python 3.2+

### Compilation
To produce an output PDF,
* Run 'pdflatex main.tex'
* Run 'pythontex main.tex'
* Run 'pdflatex main.tex' a second time.
The output file is main.pdf. 
