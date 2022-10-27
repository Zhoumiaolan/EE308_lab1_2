# Programming specifications

> The specification references:

[https://zh-google-styleguide.readthedocs.io/en/latest/google-cpp-styleguide/contents/](https://zh-google-styleguide.readthedocs.io/en/latest/google-cpp-styleguide/contents/)

## Indentation

Use 1 Tab (equals to 4 white spaces) for indentation.

## Variable Name
The runtime of this program is all lowercase and well-defined for variable names, which means that the reader can understand the representation from its name. Each word in the variable should be separated by an "_".

Examples:

```cpp
int count_keywords = 0;
int count_switch = 0;
int count_case = 0;
```

## Maximum number of characters per line

In this case, 80 is the maximum number of characters of a line.

## Maximum number of function lines

The lines number of each function should not exceed 40.

## Function and class naming


Typically, function and class names begin with a capital letter and are not underlined.
 Examples:

```cpp
void UserInterfaceHiddenCode(string path, int level);
void CountKeywords(fstream& fName);
void CountSwitch();
void CountSelectionTotal();
void CountIfElseNum();
void CountIfElseifElseNum();
```

## Constant


All constants must be written in capital letters and clearly defined
 Example:
```cpp
const int KEYWORDS_LIST_NUM = 32;
```

## Blank line rule

Each function is preceded by four blank lines to make it clear to the reader. The front line for select and loop statements is usually a blank line.
Examples:

```cpp
fstream File;
	File.open(path.c_str());
// a blank line here
	if (File.fail())
	{ }
```

```cpp
void function1(){
      ...
}
// a blank line here
void function2(){
      ...
}
```

## Annotation rules

For comments about variables, the comments should be synchronized with the end of the line. In other cases, however, comments are usually written at the front of the section to be interpreted and do not contain any code.
Examples:

```cpp
int number = 0 // The variable is used to count the number of ... ...

// The funtion is to ... ...
void function1(){
...
}
```

## Space before and after operator


Unary operators follow variables without Spaces between them. Binary operators must be separated by Spaces.
Examples:

```cpp
int c = a + b;
c++;
```
