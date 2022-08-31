# Software Development 2: C with Inline Assembly

The objective of this program is to receive an input file (preferably text file) and convert/count the contents within that file using a specified argument in the command line. The result of the conversion/counting is translated into an output file called `output.txt`.

This command line tool is incredibly useful for counting the total amount of words present within the file and converting all text within a text file to uppercase and lowercase.

## Command Line Argument Explaination

The command line tool will take arguments that will be passed by the parameters of the program. For example, to convert the content within a given input file to uppercase, then write and display it within an output file, the arguments will look like: 
```bash
convert –u -i input.txt -o output.txt
```
<img width="1472" alt="image" src="https://user-images.githubusercontent.com/96035297/187043287-c65f3af8-5d95-461f-bfd7-d154afd6da89.png">

In the example shown above, the `-u` indicates that the input file content should be converted to uppercase into the output file. Other arguments include the `-l`, and `-c`. 
* `-l` indicates that the input file should be converted to lowercase
* `-c` indicates counting the words within the input file.

The input file should always be preceded by an `-i` to ensure to the program that you’ve entered a filename. The output file declaration follows the same principle, however it is preceded by an `-o`. 

<img width="1464" alt="image" src="https://user-images.githubusercontent.com/96035297/187043715-cd49d7fe-cd09-482e-8fec-2f0190e29592.png">

<img width="1471" alt="image" src="https://user-images.githubusercontent.com/96035297/187043656-95fd2e94-a0c7-41af-9a2f-37f1a00b25e5.png">

## Default Functionality

The program will continue to run if the `-i` or `-o` arguments are not included for the filenames. If there is no `-i` included, the program will prompt the user to enter a text file (from stdin) for conversion. If `-o` is not included, then the program will continue to print the results in the stdout. 

If specifiers like, `-u`, `-l`, or `-c` are not included in the command line then the program will default the contents of the input file to uppercase. 

## Recommendations

1. **Microsoft Syntax**: It’s recommended to use the Microsoft compiler as the code comprises of inline assembly 	that runs on the Microsoft syntax.
2. **Makefile**: A Makefile is a text file that describes how your program should be built (automates the builds). We’re using a Makefile to reduce the time on typing the compile command, and simple mistakes. Makefiles consists of dependencies and rules to produce a successful compilation.

<img width="1465" alt="image" src="https://user-images.githubusercontent.com/96035297/187044012-3aa39209-1059-46d0-adb3-fe6299a99ef5.png">

## Languages & Tools Utilized

<p float="left">
  <img src="https://user-images.githubusercontent.com/96035297/186022424-f96144ad-7b39-4add-a0dc-3c0ec400124f.png" height="50" width="50" />
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=c,vscode" />
  </a>
</p>
