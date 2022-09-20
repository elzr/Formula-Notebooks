# Formula Notebooks

Notebooks of formulas for my experiments in Google Sheets.

- [Formula Notebooks](#formula-notebooks)
  - [Named functions & lambdas](#named-functions--lambdas)
  - [Spatial style](#spatial-style)
  - [Why notebooks?](#why-notebooks)
  - [Files](#files)
    - [Syntax highlighting](#syntax-highlighting)

## Named functions & lambdas
Since sep2022, native custom functions have arrived to Google Sheet formulas! [Official announcement.](https://workspaceupdates.googleblog.com/2022/08/named-functions-google-sheets.html)

* Official help pages:
  * [Named functions](https://support.google.com/docs/answer/12504534?hl=en-GB)
  * [Lambda](https://support.google.com/docs/answer/12508718)
    * [Map](https://support.google.com/docs/answer/12568985)
    * [Reduce](https://support.google.com/docs/answer/12568597)
    * [ByCol](https://support.google.com/docs/answer/12571032)
    * [ByRow](https://support.google.com/docs/answer/12570930)
    * [Scan](https://support.google.com/docs/answer/12569094)
    * [MakeArray](https://support.google.com/docs/answer/12569202)

* Ben Collins
  * [Guide to named functions](https://www.benlcollins.com/spreadsheets/named-functions/)
  * [New functions in Google Sheets for 2022](https://www.benlcollins.com/spreadsheets/new-functions-in-google-sheets-2022/)

## Spatial style
Over the 2 years (2020 & 2021) I worked building dashboards for [@StJude](https://twitter.com/StJude), I developed a spatial style of programming. It was fascinating but severely stunted by the limitations of formulas. 

The only way to reuse a piece of functionality was to copy-paste its formula. If you changed the functionality, you had to manually replace every instance of your formula! It was terribly brittle & painstaking.

Sometimes you could have one formula controlling several cells with [ARRAY_FORMULA](https://support.google.com/docs/answer/3093275?hl=en), [QUERY](https://support.google.com/docs/answer/3093343?hl=en), [FILTER](https://support.google.com/docs/answer/3093197?hl=en) & [INDEX](https://support.google.com/docs/answer/3098242?hl=en). But that only worked for certain shapes of data & compute.

One could only name data through [Named Ranges](https://support.google.com/docs/answer/63175?hl=en&co=GENIE.Platform%3DDesktop). That meant that to get [the clarity of names](https://twitter.com/qntm/status/1487870941501743111) you had to output & lay out the steps of a complex computation. 

It wasn't alll bad, at its best, it looked [like this](https://twitter.com/elzr/status/1374550012869349379) and [this](https://twitter.com/elzr/status/1391494286823329797).

But what was fascinating to me about spreadsheets was being able to use the grid, the spatial arrangement of both your data and your code. Think [cellular automata](https://en.wikipedia.org/wiki/Cellular_automaton)! Think [ORCA](https://100r.co/site/orca.html)!

Anyway, with native custom functions the ceiling of this style of programming has been raised considerably. I've been having great fun playing with the style, building it up. I want to share my progress as I keep at it. Not only is it a beautiful, powerful take on computation, I believe it can be a fast way to prototype UIs.

## Why notebooks?
Because formulas can be [literate](https://en.wikipedia.org/wiki/Literate_programming)!

Because Goggle Sheets's interface for named functions strips away indenting and has no syntax highlighting (other than argument placeholders). 

With text files we can have not only indenting & syntax highlighting but comments! We can quickly look at the code of several functions AND how it has evolved through several iterations.

The text files are not executable themselves: you have to copy-paste between text-file and Google Sheets, stripping away the comments (or simply have them around, not within the formulas). Yes, it's a bit of a pain but it's worthwhile and better than the alternative of only relying on Sheets.

## Files
File format for formula notebooks: `.gse`

### Syntax highlighting
This depends on this VSCode extension: [Google Sheets Equation Syntax Hightlighter](https://marketplace.visualstudio.com/items?itemName=leonidasIIV.google-sheets-equation-syntax-hightlighter&ssr=false#overview). It has a nice [README](https://github.com/leonidasIIV/vsc_sheets_formula_extension) here on Github. Last updated on mar2020.

