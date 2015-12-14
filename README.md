Table of Contents
=================

  * [Exercise-2](#exercise-2)
    * [Game instructions](#game-instructions)
    * [Clues](#clues)
    * [Programm interface](#programm-interface)
    * [Hints](#hints)
      * [Plotting maps](#plotting-maps)
      * [Downloading files](#downloading-files)
    * [Reporting](#reporting)
    * [Deadline](#deadline)
    * [Grading](#grading)

# Exercise-2

The second exercise is a treasure hunt based on common sense and your ability to
work with files, arrays and plotting functions. In general, a treasure hunt is
one of many different types of games which can have one or more players who try
to find hidden articles, locations or places by using a series of clues.
However, this time the game takes place in the virtual world, where bytes, bits
and mainly your Python skills are important.

## Game instructions

In the following treasure hunt you have to answer short riddles concealing file
names, column names or positions. The files are written in random formats (e.g.
.csv, .npz, .nc) and their content might contain information useful for the next
clue. All files can be downloaded from
[here](http://rs.geo.tuwien.ac.at/downloads/cpa/), however, you will only be
able to download a file once knowing its correct file name. All names are
lowercase (e.g. http://rs.geo.tuwien.ac.at/downloads/cpa/filename1.csv)!

## Clues

1. Please download **filename1.csv** and read **column1** at row number **row1**,
   which will give you **filename2part1**. Prove the solution of riddle **row1**
   with a histogram.
   - **filename1.csv**: *It has 4 legs but cannot walk.*
   - **column1**: *Young I'm tall, old I'm short, I love to glow, breath is my
     foe.*
   - **row1**: *What digit is the most frequent between the numbers 1 and 1000?*

2. Please download **filename2part1_filename2part2.nc**, which is a treasure
   map. Read and plot **variable2**. Which capital city has been marked? The
   answer to this question will give you **filename3part1**.
   - **filename2part2**: *Stay hungry, stay ......, Steve Jobs*
   - **variable2**: *May the ..... be with you, Han Solo*

3. Please download **filename3part1_filename3part2.npz** and read **variable3**. In
   **row3** you will find **filename4.bin**.

   - **filename3_part2**: *What planet has the shortest year?*
   - **variable3**: *I'll be ...., Arnold Schwarzenegger*
   - **row3**: Mean of **column3** in the file **filename1.csv**.
   - **column3**: *An ..... a day keeps the doctor away!*

4. Please download **filename4.bin**. The first 107 bytes will tell you how to
   read the rest of the file. 
  
5. Finally you have to generate a HDF5 file on your own representing the final
   treasure map. The file needs to have 3 variables: **longitude**, **latitude** and
   **dataset**. You should be able to generate a plot from your file and find the
   name of the island where the treasure can be found.

   - **longitude**: data can be found in **filename1.csv** in **column5**
   - **latitude**: data can be found in **filename3.npz** in **variable5a**
   - **dataset**: data can be found in **filename4.bin** in **variable5b**
   - **column5**: *Alive without breath, as cold as death; never thirsty, ever
     drinking, all in mail, never clinking.*
   - **variable5a**: *What gets wetter and wetter the more it dries?*
   - **variable5b**: *What is black and white and red all over?*

## Programm interface

Try to write structured and documented programs using functions. Please respect
[PEP8](https://www.python.org/dev/peps/pep-0008/) and
[PEP20](https://www.python.org/dev/peps/pep-0020/).

## Hints

### Plotting maps

The [basemap](http://matplotlib.org/basemap/) package can be used for plotting
maps. [Here](http://matplotlib.org/basemap/users/examples.html) you can find
examples how to plot data on a map.

### Downloading files

The package [urllib2](https://docs.python.org/2/library/urllib2.html) comes with
the standard library.

## Reporting

The following is required when handing in the exercise:
- *Documented* and *executable* python source code,
- *plots* of the treasure maps and
- a *text file* with all answers.

Please .zip all files and send it to
[sebastian.hahn@geo.tuwien.ac.at](mailto:sebastian.hahn@geo.tuwien.ac.at).

## Deadline

18.01.2016 23:59

## Grading

The grade for this exercise will be based on the implementation style (30%), the
documentation of your code (30%), if the code is working (30%) and the complete
delivery of all files (code and graphics) (10%).

1. 91-100
2. 81-90
3. 66-80
4. 51-65
5. < 51
