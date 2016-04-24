flex++ and bison++ were created from flex and bison by A. Coetmeur in the 1990s.
These two programs provided seamless integration with C++, allowing developers to code actions in C++ and embed a parser and scanner within a class by private inheritance. The latter capability allows multiple scanners and parsers to be used within a single program, something that is difficult with flex and bison.

flex++ and bison++ impressed me as being well-engineered when I first discovered them, and my opinion remains undimmed today. But releases ended in 1993 and flex++ and bison++ fell out of date as C++, gcc, flex,and bison all evolved. Soon I was making hasty, on-the-fly patches whenever a new version of gcc appeared (no pre-built packages are available for my Linux distribution).
So I loaded the 1993 releases into Subversion, updated them more carefully, and offer them here.

These updated "-45" versions build cleanly under gcc 4.5 (except for [issue 1](https://code.google.com/p/flexpp-bisonpp/issues/detail?id=1)) and the generated scanners and parsers compile/link under g++ 4.5. flex++ now includes a _configure_ file as well. Also available in Downloads are the original releases and code samples from 1993.

License Note: Bison and bison++ are released under the GPL. Flex and flex++ use a modified BSD license.