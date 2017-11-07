
Convert given source code into .pdf with syntax highlighting and more features

| Build Status | Version | Downloads | Python   |
| ------------ |---------|-----------|----------|


```sh
git clone https://github.com/tushar-rishav/code2pdf.git
cd code2pdf
python setup.py install

```
Or

##### Using pip

```sh
pip install code2pdf

```
### Usage

##### A. As console app

###### Help

```sh
code2pdf -h

```
###### Usage
 ` code2pdf [-h] [-l] [-s SIZE] [-S NAME] [-v] filename [outputfile] `

###### Options

```sh
positional arguments:
  filename              absolute path of the python file
  outputfile            absolute path of the output pdf file

optional arguments:
  -h, --help            show this help message and exit
  -l, --linenos         include line numbers.
  -s SIZE, --size SIZE  PDF size. A2,A3,A4,A5 etc
  -S NAME, --style NAME
                        the style name for highlighting. Eg. emacs, vim style etc.
  -v, --version         show program's version number and exit

```
###### Available style types are

- [x] autumn
- [x] borland
- [x] bw
- [x] colorful
- [x] default
- [x] emacs
- [x] friendly
- [x] fruity
- [x] igor
- [x] manni
- [x] monokai
- [x] murphy
- [x] native
- [x] paraiso-dark
- [x] paraiso-light
- [x] pastie
- [x] perldoc
- [x] rrt
- [x] tango
- [x] trac
- [x] vim
- [x] vs
- [x] xcode

###### Example
```sh
 code2pdf -l -s a3 -S emacs ~/Code2Pdf/Code2pdf/code2pdf.py ~/Code2Pdf/Demo/demo.pdf

```
To see the demo for above check `Demo/` in github repo

##### B. As module

```py
	
from Code2pdf.code2pdf import Code2pdf
ifile,ofile,size = "test.py", "test.pdf", "A4"
pdf = Code2pdf(ifile, ofile, size)	# create the Code2pdf object
pdf.init_print()	# call print method to print pdf

```

### License
![gpl](https://cloud.githubusercontent.com/assets/7397433/9025904/67008062-3936-11e5-8803-e5b164a0dfc0.png)


