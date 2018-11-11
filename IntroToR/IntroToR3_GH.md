R markdown report for github
================

# Background

The purpose of this is to show everyone how markdown works. The first
header is called “Background”.

## This is a subheader

Here, I’ll show how to change the font style and create an itemized
list.

  - One asterisk for *italic*
      - Subitem
  - Two for **bold**
  - tildes for ~~strike through~~.

### Code chunks

#### R code

To specify a chunk of code start with `{engine, evaluate code?, show
code?...} and end with`. This is a chunk of R code. The engine is R, we
will run the code, and show the output.

``` r
HiR <- "Hi from R!!"

print(HiR)
```

    ## [1] "Hi from R!!"

#### bash code

We can also call bash codes from inside our markdown document. Here the
engine is bash, so we change the first line accordingly.

``` bash
echo 'Hi, its me again!'
```

    ## Hi, its me again!

``` bash
echo 'Hi, its me again, but this time there no output :('
```

# Show some plots

This is a plot aligned to the
left.

``` r
hist(rnorm(100, 10, 2), breaks = 20)
```

<img src="IntroToR3_GH_files/figure-gfm/plot hist-1.png" style="display: block; margin: auto auto auto 0;" />

Here’s one to the
right.

``` r
hist(rnorm(100, 10, 2), breaks = 20)
```

<img src="IntroToR3_GH_files/figure-gfm/plot hist2-1.png" style="display: block; margin: auto 0 auto auto;" />

# Displaying formulas using latex

Enclosing some latex code in one $ will produce an inline formula
\(y = x + e\). If you use two $ it will be placed beneath the text
\[ y = x + e \]

Online equation builders can be helpful for beginners check one out
[here](https://www.codecogs.com/latex/eqneditor.php).
