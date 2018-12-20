# Solving Sudoku from Correct-Image

A project to solve a Sudoku

### Input

Input You will give unsolved sudoku that is corrected already(With good views and straight col and rows)

<p align="left">
  <img src="images/sudoku_1.jpg" width="300">
</p>

### Output

The same sudoku with ready solution

<p align="left">
  <img src="images/sudoku_1_solved.jpg" width="300">
</p>

### Some rules to use this application

1. Images can not be rotated so only images with perfect rotation are processed.
2. Only images with only one Sudoku and no other artifacts can be processed.
3. The Sudoku does not have to be fullscreen as a single Sudoku can be detected and cropped.
4. Each detected Sudoku is scaled to 500x500 pixels and stored like this.

### Contents

#### sudoku_solver.py

Provides functions to solve a sudoku puzzle.

Sudokus are formatted as a string where the rows are concatenated and empty spaces are represented as "0" or as ".".

"100200040020003900907000500004000057000541000350000100003000709001400080090002006"

#### solve_sudoku_from_image.py

Takes an image of a unsolved Sudoku as input, detects the existing digits, solves the Sudoku and returns the given image with the solution filled in. The output file is stored to the same directory as the input and has "\*(image_name)\_solved" concatenated to the image name.

### Usage

```
python3 solve_sudoku_from_image.py --image <path>
```

### Libraries that are used

_OpenCV2_ is used for the image processing.

_Tesseract_ is used to detect the digits in the given image.

<p align="right">
  Done for Data Science Lesson
  Controlled by Azamat Kibekbaev
  Made Marsel Melisov
</p>
If you have any questions about project don't shy to ask me on marsel.melisov@iaau.edu.kg
