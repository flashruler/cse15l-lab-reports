# Week 5 Lab Report

# grep -i,-c,-m

Example 1: -i

Using -i in grep allows you to ignore cases when searching for a file.

In the example shown below I searched for "gibbs 1995" which returned me files that included that string regardless of the casing. its useful as it enables searching for files quickly without the need for worring about proper casing.

    jaybuens@Jays-MacBook-Pro-2 docsearch % grep -i "gibbs 1995"  technical/plos/journal*
    technical/plos/journal.pbio.0020001.txt:        output between the developing and already developed countries (Gibbs 1995; May 1997;
    technical/plos/journal.pbio.0020001.txt:        the world (Gibbs 1995; May 1997; Alonso and Fernández-Juricic 2001; Vohora and Vohora
    technical/plos/journal.pbio.0020001.txt:        (Gibbs 1995). Consequently, there are more high-profile regional publication opportunities


Example 2: -c

-c allows you to search for the number of times a string would show up in a file or collection of files.

    jaybuens@Jays-MacBook-Pro-2 docsearch % grep -c "the" technical/plos/journal.pbio.0020001.txt
    147

By doing this, it can quickly count how much a certain string would appear in a file

Example 3: -m

When using -m you add a number after it which denotes how many iterations it will search for. e.g. `-m 5` will only loop 5 times.

An example for this is when searching for specific words quickly without forcing the command to read through the entire document

    jaybuens@Jays-MacBook-Pro-2 docsearch % grep -i -m 5 "cell" technical/plos/journal.pbio.0020001.txt
        to the sciences will be an excellent investment by developing nations in terms of

# less -N, /pattern, m

Example 1: -N

The -N command in less allows the user to display line numbers when reading a file, allowing for quick reference when referring back to a line, similar to a file on an IDE.

     6         Kofi Annan, the Secretary-General of the United Nations, recentl
      6 y called attention to
      7         the clear inequalities in science between developing and develop
      7 ed countries and to the
      8         challenges of building bridges across these gaps that should bri
      8 ng the United Nations and
      9         the world scientific community closer to each other (Annan 2003)
      9 . Mr. Annan stressed the
     10         importance of reducing the inequalities in science between devel
     10 oped and developing
     11         countries, asserting that “This unbalanced distribution of scien
     11 tific activity generates
     12         serious problems not only for the scientific community in the de
     12 veloping countries, but for
     13         development itself.” Indeed, Mr. Annan's sentiments have also be
     13 en echoed recently by
     14         several scientists, who present overwhelming evidence for the di
     14 sparity in scientific

