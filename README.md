# comp40
A depository for Tufts University's Machine Structure and Assembly Programming Course (Fall 2023)

## Course Projects
1. filesofpix
2. iii
3. locality
4. arith
5. bomb
6. um (Universal Machine)
7. profiling
8. asmcoding

## Project Descriptions

In alignment with course academic integrity policies, I am unable to share my code from these projects publicly. However, I can share a description of the various projects. If you are interested and not a potential student of copm40, then feel free to reach out and I would be more than happy to share my solutions!

### filesofpix

The goal of the filesofpix program is to parse through an image and identify which rows are part of an original valid image and which have been tampered with by a supposed bad actor.
Under the premise of the assignment, all rows have been injected with non-digit ascii characters and some rows have been added with a consistent pattern of ascii characters. The program must identify the pattern in added rows, and then parse through the rows to determine which rows must be restored and which rows must be discarded. In addition, the original rows must also have all non-digit characters removed and then be written to an output image.

### iii

This program contained several portions including the implementation of a polymorphic two-dimensional unboxed array module and a two-dimensional bitmap using the Hanson UArray (unboxed array). In addition, these modules were used to build a program that removes erroneous black pixels in photocopies and a sudoku solution verifier respectively.

### locality

This program allows for the transformation of images (pgms) of any size. Implemented transformations are 90, 180, and 270-degree rotations, transposition across the upper left to bottom right diagonal, and vertical and horizontal flips. In addition, the client could specify the traversal order (column-major, row-major, and block-major order) and opt to time the transformation.

### arith

This program allows for the compression of ppm images by using discrete cosine transformations to convert RBG values to component video color space representation and then bitpacking the associated values into a custom file format. It also allows for the decompression of this image by parsing the file format, converting it back to RGB values, and writing to a ppm file format.

### bomb

This project was diffusing the binary bomb, an executable of a c program that requires specific input to avoid a function called explode_bomb. Our task was to parse through the assembly of the executable and use GDB to determine what the input was.

### um (Universal Machine)

The universal machine emulates the intel 8085 microprocessor and interprets 32-bit words to basic operations to manipulate a segmented memory. This is to allow the creation of programs that can be run on any hardware system and perform similarly. A key aspect of this assignment was finding test cases for each operation and different combinations of operations.

### profiling

The goal of this assignment was to abandon course programming standards and optimize our universal machine. We used Callgrind to analyze the assembly code of our c program to identify stress points in our program and appropriately reduce the performance time of our universal machine against several benchmarks.

### asmcoding

This assignment echoes a previous assignment in the Tufts computer science cannon: a C++ Reverse Polish Notation calculator. This project implements the same functionality as this previous assignment but in UMASM, an assembly language designed with the grammar of x86 AMD64 assembly but compatible with the Universal Machine instructions. Functionality included addition, subtraction, multiplication, division, bitwise operations, comparison, and swapping, duplicating, and deleting values on the stack.
