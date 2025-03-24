# Charis

[![][Fontbakery]](https://googlefonts.github.io/googlefonts-project-template/fontbakery/fontbakery-report.html)
[![][Universal]](https://googlefonts.github.io/googlefonts-project-template/fontbakery/fontbakery-report.html)
[![][GF Profile]](https://googlefonts.github.io/googlefonts-project-template/fontbakery/fontbakery-report.html)
[![][Shaping]](https://googlefonts.github.io/googlefonts-project-template/fontbakery/fontbakery-report.html)

[Fontbakery]: https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Fgooglefonts%2Fgooglefonts-project-template%2Fgh-pages%2Fbadges%2Foverall.json
[GF Profile]: https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Fgooglefonts%2Fgooglefonts-project-template%2Fgh-pages%2Fbadges%2FGoogleFonts.json
[Outline Correctness]: https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Fgooglefonts%2Fgooglefonts-project-template%2Fgh-pages%2Fbadges%2FOutlineCorrectnessChecks.json
[Shaping]: https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Fgooglefonts%2Fgooglefonts-project-template%2Fgh-pages%2Fbadges%2FShapingChecks.json
[Universal]: https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Fgooglefonts%2Fgooglefonts-project-template%2Fgh-pages%2Fbadges%2FUniversal.json

This project is intended to provide a free and open font family for all
current languages and writing systems that use Latin and Cyrillic scripts.
It supports almost the complete range of Unicode characters for these scripts,
including a comprehensive range of diacritics and a large set of symbols
useful for linguistics and literacy work. Smart font routines automatically
adjust the position of diacritics to support and optimize arbitrary
base+diacritic combinations.

Charis is optimized for readability in long printed documents. It is
highly readable and holds up well in less-than-ideal reproduction environments
due to its simple and robust design with strong serifs and clear features.

![Highly legible design](documentation/ProductSites-Charis2-72.jpg)
![Complete character set](americas-woman-bible-72.jpg)

## About

The Charis project is maintained by SIL Global, a global,
faith-based nonprofit that works with local communities around the world
to develop language solutions that expand possibilities for a better life.

## Building

Fonts are built automatically by GitHub Actions - take a look in the "Actions" tab for the latest build.

If you want to build fonts manually on your own computer:

* `make build` will produce font files.
* `make test` will run [FontBakery](https://github.com/googlefonts/fontbakery)'s quality assurance tests.
* `make proof` will generate HTML proof files.

The proof files and QA tests are also available automatically via GitHub Actions - look at `https://yourname.github.io/your-font-repository-name`.

## Changelog

When you update your font (new version or new release), please report all notable changes here, with a date.
[Font Versioning](https://github.com/googlefonts/gf-docs/tree/main/Spec#font-versioning) is based on semver. 
Changelog example:

### 1 Feb 2023 (SIL WSTech Team) Charis SIL version 6.200

This release is focused on adding features and glyphs, including support for over 180 additional characters mostly from Unicode 14 and 15. It does not include significant changes to line spacing, glyph widths, or kerning that might cause document reflow or layout changes - except for minor improvements to the size and weight of superscript, subscript, and modifier letters.

#### New features, including *TypeTuner Web* support

- Feature to display alternate design of clicks that sit on baseline
    - Baseline clicks (cv69)
 
- Standard 'subs' and 'sups' features for numerals. These are not supported by *TypeTuner Web*.
    - Subscript numerals (subs)
    - Superscript numerals (sups)

- Feature to automatically construct fractions when using U+002F SOLIDUS or U+2044 FRACTION SLASH. This is not supported by *TypeTuner Web*.
    - Automatic fractions (frac)

#### New character support

- Additional click (also supported by new baseline clicks feature)
    - U+2980 TRIPLE VERTICAL BAR DELIMITER

- Letters used for legacy Malayalam transliteration
    - U+1DF25 LATIN SMALL LETTER D WITH MID-HEIGHT LEFT HOOK
    - U+1DF26 LATIN SMALL LETTER L WITH MID-HEIGHT LEFT HOOK
    - U+1DF27 LATIN SMALL LETTER N WITH MID-HEIGHT LEFT HOOK
    - U+1DF28 LATIN SMALL LETTER R WITH MID-HEIGHT LEFT HOOK
    - U+1DF29 LATIN SMALL LETTER S WITH MID-HEIGHT LEFT HOOK
    - U+1DF2A LATIN SMALL LETTER T WITH MID-HEIGHT LEFT HOOK

- Letters used for Egyptological transliteration
    - U+A7BA LATIN CAPITAL LETTER GLOTTAL A
    - U+A7BB LATIN SMALL LETTER GLOTTAL A
    - U+A7BC LATIN CAPITAL LETTER GLOTTAL I
    - U+A7BD LATIN SMALL LETTER GLOTTAL I
    - U+A7BE LATIN CAPITAL LETTER GLOTTAL U
    - U+A7BF LATIN SMALL LETTER GLOTTAL U

- Combining marks
    - U+1ABF COMBINING LATIN SMALL LETTER W BELOW
    - U+1AC0 COMBINING LATIN SMALL LETTER TURNED W BELOW
    - U+1AC6 COMBINING NUMBER SIGN ABOVE
    - U+1AC7 COMBINING INVERTED DOUBLE ARCH ABOVE
    - U+1AC8 COMBINING PLUS SIGN ABOVE
    - U+1AC9 COMBINING DOUBLE PLUS SIGN ABOVE
    - U+1ACA COMBINING DOUBLE PLUS SIGN BELOW
    - U+1ACB COMBINING TRIPLE ACUTE ACCENT
    - U+1ACC COMBINING LATIN SMALL LETTER INSULAR G
    - U+1ACD COMBINING LATIN SMALL LETTER INSULAR R
    - U+1ACE COMBINING LATIN SMALL LETTER INSULAR T
    - U+1DDA COMBINING LATIN SMALL LETTER G
    - U+1DDC COMBINING LATIN SMALL LETTER K
    - U+1DFC COMBINING DOUBLE INVERTED BREVE BELOW

- Combining marks that are not recommended for normal use and may not combine well with letters. Precomposed characters that include the hook should be used instead except in rare cases.
    - U+0321 COMBINING PALATALIZED HOOK BELOW
    - U+0322 COMBINING RETROFLEX HOOK BELOW

- Modifier letters and symbols
    - U+A7F2 MODIFIER LETTER CAPITAL C
    - U+A7F3 MODIFIER LETTER CAPITAL F
    - U+A7F4 MODIFIER LETTER CAPITAL Q
    - U+AB69 MODIFIER LETTER SMALL TURNED W
    - U+AB6A MODIFIER LETTER LEFT TACK
    - U+AB6B MODIFIER LETTER RIGHT TACK
    - U+10780 MODIFIER LETTER SMALL CAPITAL AA
    - U+10781 MODIFIER LETTER SUPERSCRIPT TRIANGULAR COLON
    - U+10782 MODIFIER LETTER SUPERSCRIPT HALF TRIANGULAR COLON
    - U+10784 MODIFIER LETTER SMALL CAPITAL B
    - U+10785 MODIFIER LETTER SMALL B WITH HOOK
    - U+10787 MODIFIER LETTER SMALL DZ DIGRAPH
    - U+10788 MODIFIER LETTER SMALL DZ DIGRAPH WITH RETROFLEX HOOK
    - U+10789 MODIFIER LETTER SMALL DZ DIGRAPH WITH CURL
    - U+1078A MODIFIER LETTER SMALL DEZH DIGRAPH
    - U+1078B MODIFIER LETTER SMALL D WITH TAIL
    - U+1078C MODIFIER LETTER SMALL D WITH HOOK
    - U+1078D MODIFIER LETTER SMALL D WITH HOOK AND TAIL
    - U+10790 MODIFIER LETTER SMALL FENG DIGRAPH
    - U+10792 MODIFIER LETTER SMALL CAPITAL G
    - U+10793 MODIFIER LETTER SMALL G WITH HOOK
    - U+10794 MODIFIER LETTER SMALL CAPITAL G WITH HOOK
    - U+10796 MODIFIER LETTER SMALL CAPITAL H
    - U+10797 MODIFIER LETTER SMALL HENG WITH HOOK
    - U+10798 MODIFIER LETTER SMALL DOTLESS J WITH STROKE AND HOOK
    - U+10799 MODIFIER LETTER SMALL LS DIGRAPH
    - U+1079A MODIFIER LETTER SMALL LZ DIGRAPH
    - U+1079B MODIFIER LETTER SMALL L WITH BELT
    - U+1079C MODIFIER LETTER SMALL CAPITAL L WITH BELT
    - U+1079D MODIFIER LETTER SMALL L WITH RETROFLEX HOOK AND BELT
    - U+1079E MODIFIER LETTER SMALL LEZH
    - U+1079F MODIFIER LETTER SMALL LEZH WITH RETROFLEX HOOK
    - U+107A1 MODIFIER LETTER SMALL TURNED Y WITH BELT
    - U+107A4 MODIFIER LETTER SMALL CLOSED OMEGA
    - U+107A5 MODIFIER LETTER SMALL Q
    - U+107A6 MODIFIER LETTER SMALL TURNED R WITH LONG LEG
    - U+107A7 MODIFIER LETTER SMALL TURNED R WITH LONG LEG AND RETROFLEX HOOK
    - U+107A8 MODIFIER LETTER SMALL R WITH TAIL
    - U+107A9 MODIFIER LETTER SMALL R WITH FISHHOOK
    - U+107AA MODIFIER LETTER SMALL CAPITAL R
    - U+107AB MODIFIER LETTER SMALL TC DIGRAPH WITH CURL
    - U+107AC MODIFIER LETTER SMALL TS DIGRAPH
    - U+107AD MODIFIER LETTER SMALL TS DIGRAPH WITH RETROFLEX HOOK
    - U+107AE MODIFIER LETTER SMALL TESH DIGRAPH
    - U+107AF MODIFIER LETTER SMALL T WITH RETROFLEX HOOK
    - U+107B0 MODIFIER LETTER SMALL V WITH RIGHT HOOK
    - U+107B3 MODIFIER LETTER GLOTTAL STOP WITH STROKE
    - U+107B4 MODIFIER LETTER REVERSED GLOTTAL STOP WITH STROKE
    - U+107B5 MODIFIER LETTER BILABIAL CLICK
    - U+107B6 MODIFIER LETTER DENTAL CLICK
    - U+107B7 MODIFIER LETTER LATERAL CLICK
    - U+107B8 MODIFIER LETTER ALVEOLAR CLICK
    - U+107B9 MODIFIER LETTER RETROFLEX CLICK WITH RETROFLEX HOOK
    - U+107BA MODIFIER LETTER SMALL S WITH CURL

- Cyrillic modifier letters, subscripts, and combining marks
    - U+1E030 MODIFIER LETTER CYRILLIC SMALL A
    - U+1E031 MODIFIER LETTER CYRILLIC SMALL BE
    - U+1E032 MODIFIER LETTER CYRILLIC SMALL VE
    - U+1E033 MODIFIER LETTER CYRILLIC SMALL GHE
    - U+1E034 MODIFIER LETTER CYRILLIC SMALL DE
    - U+1E035 MODIFIER LETTER CYRILLIC SMALL IE
    - U+1E036 MODIFIER LETTER CYRILLIC SMALL ZHE
    - U+1E037 MODIFIER LETTER CYRILLIC SMALL ZE
    - U+1E038 MODIFIER LETTER CYRILLIC SMALL I
    - U+1E039 MODIFIER LETTER CYRILLIC SMALL KA
    - U+1E03A MODIFIER LETTER CYRILLIC SMALL EL
    - U+1E03B MODIFIER LETTER CYRILLIC SMALL EM
    - U+1E03C MODIFIER LETTER CYRILLIC SMALL O
    - U+1E03D MODIFIER LETTER CYRILLIC SMALL PE
    - U+1E03E MODIFIER LETTER CYRILLIC SMALL ER
    - U+1E03F MODIFIER LETTER CYRILLIC SMALL ES
    - U+1E040 MODIFIER LETTER CYRILLIC SMALL TE
    - U+1E041 MODIFIER LETTER CYRILLIC SMALL U
    - U+1E042 MODIFIER LETTER CYRILLIC SMALL EF
    - U+1E043 MODIFIER LETTER CYRILLIC SMALL HA
    - U+1E044 MODIFIER LETTER CYRILLIC SMALL TSE
    - U+1E045 MODIFIER LETTER CYRILLIC SMALL CHE
    - U+1E046 MODIFIER LETTER CYRILLIC SMALL SHA
    - U+1E047 MODIFIER LETTER CYRILLIC SMALL YERU
    - U+1E048 MODIFIER LETTER CYRILLIC SMALL E
    - U+1E049 MODIFIER LETTER CYRILLIC SMALL YU
    - U+1E04B MODIFIER LETTER CYRILLIC SMALL SCHWA
    - U+1E04C MODIFIER LETTER CYRILLIC SMALL BYELORUSSIAN-UKRAINIAN I
    - U+1E04D MODIFIER LETTER CYRILLIC SMALL JE
    - U+1E04E MODIFIER LETTER CYRILLIC SMALL BARRED O
    - U+1E04F MODIFIER LETTER CYRILLIC SMALL STRAIGHT U
    - U+1E050 MODIFIER LETTER CYRILLIC SMALL PALOCHKA
    - U+1E051 CYRILLIC SUBSCRIPT SMALL LETTER A
    - U+1E052 CYRILLIC SUBSCRIPT SMALL LETTER BE
    - U+1E053 CYRILLIC SUBSCRIPT SMALL LETTER VE
    - U+1E054 CYRILLIC SUBSCRIPT SMALL LETTER GHE
    - U+1E055 CYRILLIC SUBSCRIPT SMALL LETTER DE
    - U+1E056 CYRILLIC SUBSCRIPT SMALL LETTER IE
    - U+1E057 CYRILLIC SUBSCRIPT SMALL LETTER ZHE
    - U+1E058 CYRILLIC SUBSCRIPT SMALL LETTER ZE
    - U+1E059 CYRILLIC SUBSCRIPT SMALL LETTER I
    - U+1E05A CYRILLIC SUBSCRIPT SMALL LETTER KA
    - U+1E05B CYRILLIC SUBSCRIPT SMALL LETTER EL
    - U+1E05C CYRILLIC SUBSCRIPT SMALL LETTER O
    - U+1E05D CYRILLIC SUBSCRIPT SMALL LETTER PE
    - U+1E05E CYRILLIC SUBSCRIPT SMALL LETTER ES
    - U+1E05F CYRILLIC SUBSCRIPT SMALL LETTER U
    - U+1E060 CYRILLIC SUBSCRIPT SMALL LETTER EF
    - U+1E061 CYRILLIC SUBSCRIPT SMALL LETTER HA
    - U+1E062 CYRILLIC SUBSCRIPT SMALL LETTER TSE
    - U+1E063 CYRILLIC SUBSCRIPT SMALL LETTER CHE
    - U+1E064 CYRILLIC SUBSCRIPT SMALL LETTER SHA
    - U+1E065 CYRILLIC SUBSCRIPT SMALL LETTER HARD SIGN
    - U+1E066 CYRILLIC SUBSCRIPT SMALL LETTER YERU
    - U+1E067 CYRILLIC SUBSCRIPT SMALL LETTER GHE WITH UPTURN
    - U+1E068 CYRILLIC SUBSCRIPT SMALL LETTER BYELORUSSIAN-UKRAINIAN I
    - U+1E069 CYRILLIC SUBSCRIPT SMALL LETTER DZE
    - U+1E06A CYRILLIC SUBSCRIPT SMALL LETTER DZHE
    - U+1E06B MODIFIER LETTER CYRILLIC SMALL ES WITH DESCENDER
    - U+1E06D MODIFIER LETTER CYRILLIC SMALL STRAIGHT U WITH STROKE
    - U+1E08F COMBINING CYRILLIC SMALL LETTER BYELORUSSIAN-UKRAINIAN I

- Miscellaneous letters
    - U+A7C7 LATIN CAPITAL LETTER D WITH SHORT STROKE OVERLAY
    - U+A7C8 LATIN SMALL LETTER D WITH SHORT STROKE OVERLAY
    - U+A7C9 LATIN CAPITAL LETTER S WITH SHORT STROKE OVERLAY
    - U+A7CA LATIN SMALL LETTER S WITH SHORT STROKE OVERLAY
    - U+AB66 LATIN SMALL LETTER DZ DIGRAPH WITH RETROFLEX HOOK
    - U+AB67 LATIN SMALL LETTER TS DIGRAPH WITH RETROFLEX HOOK
    - U+AB68 LATIN SMALL LETTER TURNED R WITH MIDDLE TILDE

- Symbols
    - U+2031 PER TEN THOUSAND SIGN
    - U+203D INTERROBANG
    - U+203E OVERLINE
    - U+2042 ASTERISM
    - U+204A TIRONIAN SIGN ET
    - U+20C0 SOM SIGN
    - U+218A TURNED DIGIT TWO
    - U+218B TURNED DIGIT THREE
    - U+21B6 ANTICLOCKWISE TOP SEMICIRCLE ARROW
    - U+21B7 CLOCKWISE TOP SEMICIRCLE ARROW
    - U+21BA ANTICLOCKWISE OPEN CIRCLE ARROW
    - U+21BB CLOCKWISE OPEN CIRCLE ARROW
    - U+2215 DIVISION SLASH
    - U+2221 MEASURED ANGLE
    - U+2227 LOGICAL AND
    - U+2228 LOGICAL OR
    - U+226E NOT LESS-THAN
    - U+226F NOT GREATER-THAN
    - U+2318 PLACE OF INTEREST SIGN
    - U+25C9 FISHEYE
    - U+25CB WHITE CIRCLE
    - U+2610 BALLOT BOX
    - U+2611 BALLOT BOX WITH CHECK
    - U+2612 BALLOT BOX WITH X
    - U+2639 WHITE FROWNING FACE
    - U+263A WHITE SMILING FACE
    - U+2713 CHECK MARK
    - U+2717 BALLOT X
    - U+27C2 PERPENDICULAR
    - U+2AFD DOUBLE SOLIDUS OPERATOR
    - U+2E3E WIGGLY VERTICAL LINE
    - U+1F12F COPYLEFT SYMBOL
    - U+1F610 NEUTRAL FACE

#### Improvements and fixes

- Kayan diacritics feature (cv79) now supported by TypeTuner Web

- Combining letters, modifier letters, superscripts, and subscripts have been made more consistent in size and weight

- Encoding fixed for U+1078E MODIFIER LETTER SMALL REVERSED E

- Size increased for:
    - U+02BE MODIFIER LETTER RIGHT HALF RING
    - U+02BF MODIFIER LETTER LEFT HALF RING
    - U+02D2 MODIFIER LETTER CENTRED RIGHT HALF RING
    - U+02D3 MODIFIER LETTER CENTRED LEFT HALF RING

- U+00AA FEMININE ORDINAL INDICATOR is now included in single-story/double-story features

- The combination of U+0079 LATIN SMALL LETTER Y and U+0328 COMBINING OGONEK forms a ligature

- Small cap form corrected for U+A78D LATIN CAPITAL LETTER TURNED H / U+0265 LATIN SMALL LETTER TURNED H

- U+0328 COMBINING OGONEK repositioned to middle leg of U+006D LATIN SMALL LETTER M

- Diacritic positioning improved for U+006A LATIN SMALL LETTER J

- Diacritic positioning improved for U+2183 ROMAN NUMERAL REVERSED ONE HUNDRED 

- Position of dot changed for U+1E23 LATIN SMALL LETTER H WITH DOT ABOVE

#### Notes

- The next major version (7) will address some complex pending issues and features and may include substantial changes to line spacing, glyph metrics, kerning, and even font family structure. If you have any requests for future versions please contact us as soon as possible. 

### 9 Feb 2022 (SIL WSTech Team) Charis SIL version 6.101

This is a maintenance release primarily focused on making the v6 fonts available on *TypeTuner Web*.

#### New

- The fonts now support SIL *TypeTuner*. Customized fonts can be created at *TypeTuner Web* (https://scripts.sil.org/ttw/fonts2go.cgi)

- New `locl` OpenType feature that supports Macedonian (MKD/mk) Cyrillic alternates

- Serbian and Macedonian alternates are also available through a new OpenType feature (cv84) for applications that do not support language-specific `locl` features

- Characters have been added to support Unicode versions up to 14.0.0 (more to be added in future releases):
    - U+A7C4 LATIN CAPITAL LETTER C WITH PALATAL HOOK
    - U+A7C5 LATIN CAPITAL LETTER S WITH HOOK
    - U+1DF00 LATIN SMALL LETTER FENG DIGRAPH WITH TRILL
    - U+1DF01 LATIN SMALL LETTER REVERSED SCRIPT G
    - U+1DF02 LATIN LETTER SMALL CAPITAL TURNED G
    - U+1DF03 LATIN SMALL LETTER REVERSED K
    - U+1DF05 LATIN SMALL LETTER LEZH WITH RETROFLEX HOOK
    - U+1DF07 LATIN SMALL LETTER REVERSED ENG
    - U+1DF09 LATIN SMALL LETTER T WITH HOOK AND RETROFLEX HOOK
    - U+1DF0A LATIN LETTER RETROFLEX CLICK WITH RETROFLEX HOOK
    - U+1DF0B LATIN SMALL LETTER ESH WITH DOUBLE BAR
    - U+1DF0C LATIN SMALL LETTER ESH WITH DOUBLE BAR AND CURL
    - U+1DF0D LATIN SMALL LETTER TURNED T WITH CURL
    - U+1DF0E LATIN LETTER INVERTED GLOTTAL STOP WITH CURL
    - U+1DF0F LATIN LETTER STRETCHED C WITH CURL
    - U+1DF10 LATIN LETTER SMALL CAPITAL TURNED K
    - U+1DF11 LATIN SMALL LETTER L WITH FISHHOOK
    - U+1DF12 LATIN SMALL LETTER DEZH DIGRAPH WITH PALATAL HOOK
    - U+1DF13 LATIN SMALL LETTER L WITH BELT AND PALATAL HOOK
    - U+1DF14 LATIN SMALL LETTER ENG WITH PALATAL HOOK
    - U+1DF15 LATIN SMALL LETTER TURNED R WITH PALATAL HOOK
    - U+1DF16 LATIN SMALL LETTER R WITH FISHHOOK AND PALATAL HOOK
    - U+1DF17 LATIN SMALL LETTER TESH DIGRAPH WITH PALATAL HOOK
    - U+1DF19 LATIN SMALL LETTER DEZH DIGRAPH WITH RETROFLEX HOOK
    - U+1DF1A LATIN SMALL LETTER I WITH STROKE AND RETROFLEX HOOK
    - U+1DF1B LATIN SMALL LETTER O WITH RETROFLEX HOOK
    - U+1DF1C LATIN SMALL LETTER TESH DIGRAPH WITH RETROFLEX HOOK
    - U+1DF1D LATIN SMALL LETTER C WITH RETROFLEX HOOK
    - U+1DF1E LATIN SMALL LETTER S WITH CURL
    
#### Improved

- The special-purpose modified fonts have been updated to be based on the current version. These are available at https://software.sil.org/lcgfonts/download/ and include *Literacy* and *Compact* versions.

- U+02DE MODIFIER LETTER RHOTIC HOOK position improved with modifier vowels: 
    - U+02B8 MODIFIER LETTER SMALL Y
    - U+1D53 MODIFIER LETTER SMALL OPEN O
    - U+1D5A MODIFIER LETTER SMALL TURNED M
    - U+1DBA MODIFIER LETTER SMALL TURNED V

- Design improved for these characters:
    - U+0184 LATIN CAPITAL LETTER TONE SIX
    - U+0185 LATIN SMALL LETTER TONE SIX

- The small caps feature (smcp) now supports more characters

- The spacing of Serbian italic alternates has been improved

#### Changed encoding

- The following characters were in the SIL PUA but have now been given Unicode assignments. The SIL PUA characters are now deprecated:
    - U+A7C6 LATIN CAPITAL LETTER Z WITH PALATAL HOOK (was U+F234)
    - U+10783 MODIFIER LETTER SMALL AE (was U+F1A1)
    - U+1078F MODIFIER LETTER SMALL CLOSED REVERSED OPEN E (was U+F1A4)
    - U+10791 MODIFIER LETTER SMALL RAMS HORN (was U+F1B5)
    - U+10795 MODIFIER LETTER SMALL H WITH STROKE (was U+F1BC)
    - U+107A0 MODIFIER LETTER SMALL TURNED Y (was U+F1CE)
    - U+107A2 MODIFIER LETTER SMALL O WITH STROKE (was U+F1AB)
    - U+107A3 MODIFIER LETTER SMALL CAPITAL OE (was U+F1AE)
    - U+107B2 MODIFIER LETTER SMALL CAPITAL Y (was U+F1B4)
    - U+1088E NABATAEAN LETTER FINAL KAPH (was U+F1A3)
    - U+1DF04 LATIN LETTER SMALL CAPITAL L WITH BELT (was U+F268)
    - U+1DF06 LATIN SMALL LETTER TURNED Y WITH BELT (was U+F267)
    - U+1DF08 LATIN SMALL LETTER TURNED R WITH LONG LEG AND RETROFLEX HOOK (was U+F269)
    - U+1DF18 LATIN SMALL LETTER EZH WITH PALATAL HOOK (was U+F235)

### 2 July 2021 (SIL WSTech Team) Charis SIL version 6.001

- Reverted font Postscript name to that used in v5 and earlier to avoid
problems with unrecognized fonts when opening older documents.

### 29 Jun 2021 (SIL WSTech Team) Charis SIL version 6.000

***Note that this is a major upgrade that may cause document reflow as
some glyphs widths have changed and some features have been removed.***

#### Removed

- **Removed DSIGs added in version 5.000.** These have now been removed
to reflect current best practice font development guidance. Adobe InDesign
will complain that fonts cannot be found if a document last saved with
version 5.000 is opened with version 5.960 or later installed. It will be
necessary to find/replace the fonts in the document using the command in
the Type menu. Please also look over the document carefully to note any
places where changes in the fonts have affected letterforms or spacing.

- **Graphite has been removed.** Application and OS support for OpenType
has greatly improved, so the need for Graphite in this font family is
greatly reduced. *If this affects you, and you find that OpenType does 
not provide sufficient support for your needs, please contact us right
away.*  

- Removed the "Show Invisibles" feature.

- Removed support for nine-level pitch contours. These will be replaced
by a standalone pitch contours font in the future.

#### Added

Characters added to support Unicode versions 7.0-13.0, including feature
support (e.g. small caps) where appropriate:

- U+03D1 GREEK THETA SYMBOL
- U+03F4 GREEK CAPITAL THETA SYMBOL
- U+1AB0 COMBINING DOUBLED CIRCUMFLEX ACCENT
- U+1AB1 COMBINING DIAERESIS-RING
- U+1AB2 COMBINING INFINITY
- U+1AB3 COMBINING DOWNWARDS ARROW
- U+1AB4 COMBINING TRIPLE DOT
- U+1AB5 COMBINING X-X BELOW
- U+1AB6 COMBINING WIGGLY LINE BELOW
- U+1AB7 COMBINING OPEN MARK BELOW
- U+1AB8 COMBINING DOUBLE OPEN MARK BELOW
- U+1AB9 COMBINING LIGHT CENTRALIZATION STROKE BELOW
- U+1ABA COMBINING STRONG CENTRALIZATION STROKE BELOW
- U+1DF5 COMBINING UP TACK ABOVE
- U+203B REFERENCE MARK
- U+20BE LARI SIGN
- U+20BF BITCOIN SIGN
- U+27E8 MATHEMATICAL LEFT ANGLE BRACKET
- U+27E9 MATHEMATICAL RIGHT ANGLE BRACKET
- U+2E13 DOTTED OBELOS
- U+2E14 DOWNWARDS ANCORA
- U+2E17 DOUBLE OBLIQUE HYPHEN
- U+2E22 TOP LEFT HALF BRACKET
- U+2E23 TOP RIGHT HALF BRACKET
- U+2E24 BOTTOM LEFT HALF BRACKET
- U+2E25 BOTTOM RIGHT HALF BRACKET
- U+A78F LATIN LETTER SINOLOGICAL DOT
- U+A7AE LATIN CAPITAL LETTER SMALL CAPITAL I
- U+A7AF LATIN LETTER SMALL CAPITAL Q
- U+A7B3 LATIN CAPITAL LETTER CHI
- U+A7B4 LATIN CAPITAL LETTER BETA
- U+A7B5 LATIN SMALL LETTER BETA
- U+A7B6 LATIN CAPITAL LETTER OMEGA
- U+A7B7 LATIN SMALL LETTER OMEGA
- U+A7B8 LATIN CAPITAL LETTER U WITH STROKE
- U+A7B9 LATIN SMALL LETTER U WITH STROKE
- U+AB30 LATIN SMALL LETTER BARRED ALPHA
- U+AB53 LATIN SMALL LETTER CHI
- U+AB5C MODIFIER LETTER SMALL HENG
- U+AB5E MODIFIER LETTER SMALL L WITH MIDDLE TILDE
- U+F26E CAPITAL RAMS HORN (in SIL PUA)

#### New

- First release that uses a UFO-based design and production workflow
    - All sources are in open formats
    - Build toolkit and workflow is completely open-source
    - See https://silnrsi.github.io/silfontdev/en-US/Introduction.html

- Web fonts are provided in both WOFF and WOFF2 formats

- Applied new hinting techniques to try to improve screen rendering on Windows

- All-new documentation in HTML and PDF formats

- Features for controlling literacy forms of a and g separately
    - Literacy a alternates (ss02)
    - Literacy g alternates (ss03)

- Feature to support side-by-side rendering of U+0300 plus U+0301
    - Kayan diacritics (cv79)

- Tone letter features (cv91 & cv92) now supported through OpenType

#### Fixes

- Width of typographic spaces have been made more consistent to reflect
common publishing industry usage. Note that this may affect line and page
lengths. Affected spaces:

    - U+2000 EN QUAD (made width consistent)
    - U+2001 EM QUAD (made width consistent)
    - U+2007 FIGURE SPACE (made wider to match numerals in all styles)
    - U+2009 THIN SPACE (made narrower)
    - U+202F NARROW NO-BREAK SPACE (made narrower)

- Fixed some small capital correspondences, including added support for clicks

- Fixed problems with spacing of tone letters

- Fixed missing or distorted Vietnamese composite glyphs

- Fixed miscellaneous distorted glyphs

- Improved miscellaneous anchor positions, including the position of diacritics 
below glyphs with macrons below (e.g. U+1E0F LATIN SMALL LETTER D WITH LINE BELOW)

- Improved position of diacritics for superscripts and modifier letters
(including cedilla, ogonek, rhotic hook)

- Fixes and improvements to various glyphs:
    - U+0037 DIGIT SEVEN (spacing)
    - U+01E5 LATIN SMALL LETTER G WITH STROKE (bar position on single-story variant)
    - U+02D6 MODIFIER LETTER PLUS SIGN (size)
    - U+02DF MODIFIER LETTER CROSS ACCENT (size)
    - U+02E4 MODIFIER LETTER SMALL REVERSED GLOTTAL STOP (form)
    - U+033B COMBINING SQUARE BELOW (more rectangular)
    - U+1AB3 COMBINING DOWNWARDS ARROW (position fixes since beta 1)
    - U+1D02 LATIN SMALL LETTER TURNED AE (made double-story in italic)
    - U+1D15 LATIN LETTER SMALL CAPITAL OU (form)
    - U+1D46 MODIFIER LETTER SMALL TURNED AE (made double-story in italic)
    - U+1D77 LATIN SMALL LETTER TURNED G (position)
    - U+1D78 MODIFIER LETTER CYRILLIC EN (form)
    - U+1EFC LATIN CAPITAL LETTER MIDDLE-WELSH V
    - U+A76A LATIN CAPITAL LETTER ET
    - U+A76B LATIN SMALL LETTER ET
    - U+A76C LATIN CAPITAL LETTER IS
    - U+A76D LATIN SMALL LETTER IS
    - U+A77F LATIN SMALL LETTER TURNED INSULAR G (position)
    - U+A7F8 MODIFIER LETTER CAPITAL H WITH STROKE (form)
    - U+A7FA LATIN LETTER SMALL CAPITAL TURNED M (italic)

#### Known issues

- There is no support for TypeTuner or TypeTuner Web. We hope to add that support soon.

- There are no regional subsets. Please contact us if these are a priority for you and describe how you use them. We are reassessing whether to provide these subsets. With current web technology and WOFF2 compression most uses can be met equally well with the full fonts.

### 27 Oct 2014 (SIL NRSI team) Charis SIL version 5.000
- Added Stylistic Sets to the font for OpenType support 
	of previously Graphite-only features
- Added Character Variants to the font for OpenType support 
	of previously Graphite-only features
- Added Serbian feature when Serbian language is turned on
- Added hook D variant feature (for U+018A/U+0257)
- Removed "Show deprecated PUA" feature
- Removed "Romanian-style diacritics" feature 
  (because glyphs are now encoded)
- Removed "Diacritic selection" feature
- Added U+039E, U+03BC, U+03C6 and U+03C9 in the Greek and Coptic block
- Added U+0528..U+052F in the Cyrillic Supplement block
- Added U+2041 in the General Punctuation block
- Added U+2095..U+209C in the Superscripts and Subscripts block
- Added U+20B6..U+20BD in the Currency Symbols block
- Added U+210C, U+2113, U+2117, U+212D, U+2135, U+214F in the 
  Letterlike Symbols block
- Added U+2150..U+2152 and U+2189 in the Number Forms block
- Added U+2226, U+2234..U+2235, U+2262, U+2282..U+2287 in the 
  Mathematical Operators block
- Added U+2640, U+2642, U+266D, U+266F in the Miscellaneous Symbols block
- Added U+27E8..U+27E9 in the Miscellaneous Mathematical Symbols-A block
- Added U+2C7E..U+2C7F in the Latin Extended-C block
- Added U+2C88 in the Coptic block
- Added U+2E00..U+2E0D, U+2E3A..U+2E3B in the Supplemental 
  Punctuation block
- Added U+A736..U+A73F, U+A742..U+A74D, U+A750..U+A787, U+A790..U+A7AD, 
  U+A7B0..U+A7B1, U+A7F7..U+A7FA in the Latin Extended-D block. 
  These were also added to relevant features.
- Added U+A92E in the Kayah Li block (to support the Kayah Li language 
  when using the Roman script)
- Added U+AB64..U+AB65 in the Latin Extended-E block
- Added U+1D40C, U+1D504..U+1D505, U+1D50A, U+1D50E..U+1D50F, U+1D514, 
  U+1D516..U+1D517, U+1D519 in the Mathematical Alphanumeric Symbols block
- Added PUA characters U+F26C (curl J) and U+F26D (left-hook b)
- Characters in our PUA that were added to Unicode have had their 
  codepoints updated:
  F1AD>A7F9, F266>A78E, F26B>A78D, F32C>0526, F32D>0527, F17B>1DFD, F209>2C70
- These PUA characters were deprecated (now white on black glyphs): 
  U+F17B, U+F1AD, U+F209, U+F247, U+F248, U+F266, U+F26B, U+F32C, U+F32D
- Deleted U+0149 as it is officially deprecated in Unicode
- Added support for shorter macrons under narrow letters (i,l,r,t).
  (This only works for Graphite or using precomposed characters in OpenType.)
- Made it possible for saltillo characters (U+A78B and U+A78C) to "carry" 
  diacritics
- Improved design of U+A722..U+A725 and U+A78D
- Refactored all cedilla positioning
- Removal of unneeded duplicate glyphs (because of improvements in smart 
  font code)
- Bug fix in Graphite code to allow for simultaneous selection of Vietnamese 
  alternates and Small Caps
- Bug fix in Graphite code to allow for simultaneous selection of Ogonek 
  alternates and Small Caps
- Improved hinting
- Significant size, position and metric changes made to Subscript and Superscript 
  parentheses, plus, minus, equals.
- Size of guillomets (U+00AB U+00BB U+2039 U+203A) modified to match the font. 
  Metrics were not changed.
- Arrowhead design of U+21A8 modified to match the other arrows
- Placement of Ogonek revisited
- Slight modification to positioning of U+0361 and U+035C in Italic and Bold Italic
- Changed the strongly curved hooks on Cyrillic U+04C3..U+04C4, U+04C7..U+04C8, 
  U+04FC..U+04FD, U+0512..U+0513 to be more consistent with other hooks
- Modified Cyrillic italic versions of U+04AF, U+04B1, U+04B5, U+04BC, U+04BE, U+04D8
- Modified design of U+A78D to be more curved and less squared
- Changed postscript names for U+0218 and U+0219
- Changed postscript names for U+2203, U+232A and U+2329
- "Hide tone contour staves" feature now works with single tonebar
- U+1DBF now follows weight and italic changes
- Allowed combining marks to render properly with U+02D0
- Removed AAT support

### 10 Jun 2013 (SIL NRSI team) Charis SIL version 4.114
- optimized Graphite code for faster processing of plain ASCII text

### 1 Aug 2012 (SIL NRSI team) Charis SIL version 4.112
- Changed Graphite feature identifiers from integers to 4-character 
  alphanumeric tags (no other changes)
  
### 12 Sep 2011 (SIL NRSI team) Charis SIL version 4.110
- Removed the VDMX table
- Changed version number (using ttfsetver)

### 25 Aug 2011 (SIL NRSI team) Charis SIL version 4.108
- Double-encoded the SIL PUA characters which were added to Unicode 5.2 and 6.0
  (using ttfremap)
- Encoded 1D29 (using ttfremap)
- Corrected problem with coverage tables (using ttfsortcover)
- Changed version number (using ttfsetver)
- Added device metric tables
- Added an empty dsig table

### 05 May 2009 (Alan Ward) Charis SIL version 4.106
- TypeTuner (Silt) table changed so that line metrics from legacy fonts
  can be imported

### 20 Mar 2009 (SIL NRSI team) Charis SIL version 4.106
- Added support for Unicode 5.1 Latin and Cyrillic additions
- Other characters added: 0462, 0463, 0474, 0475, 0524, 0525, 20E5, 2203, 2204,
  231C..U+231F, 2329, 232A, 239B..23AD, A722..U+A725
- Added PUA characters F26B, F32C, F32D
- Design changes: 002F, 00A1, 00BF, 02D0, 02ED, 02FF, 034B, 04A8, 04A9, 04BC,
  04BD, 04BE, 04BF, 04E0, 04E1, 045F, 04AA, 04AB, F208, F209, 0358
- Fixed attachment points on 1D68, 1D69, 1D6A, 04FA, 04FB, fi and fl ligatures
- Fixed collision issues for Vietnamese glyphs 'with horn'
- Fixed advance of t-caron
- Feature modifications:
    * new alternates added to feature ID 1033 and renamed from Small v-hook
      alternate
      to V-hook alternates
    * new alternate U+2C65 LATIN SMALL LETTER A WITH STROKE added to
      Literacy alternates feature
    * default for Diacritic selection was changed from "on" to "off"
      (by request of FieldWorks team)
- Added new features:
    * Small Caps
    * Non-European caron alternates
    * Capital B-hook alternate
    * Show deprecated PUA
- Slant italic bug fixed (dot on i was not disappearing with combining marks)
- Removal of about 700 unused glyphs (including precomposed chao tone letters
  which were no longer needed since these are now dynamically created)
- Fixed issues: kern table error, usMaxContext and yMax errors
- Several OpenType issues fixed
- Graphite reordering bug fixed
- Automated AAT build process
- Changed OFL license to version 1.1
  
### 9 May 2008 (SIL NRSI team) Charis SIL version 4.104
- Double-encoded the SIL PUA characters which were added to Unicode 5.1 
  (using ttfremap)
- Changed version number (using ttfsetver)

### 16 Aug 2007 (SIL NRSI team) Charis SIL version 4.102
- Modified the OpenType features so that InDesign's built-in small caps work

### 31 Jan 2007 (SIL NRSI team) Charis SIL version 4.100
- Added PUA character F26A
- Added 2308, 2309
- Removed Cyrillic italic alternates feature and added those 3 characters to the
  slant italic specials feature
- Fixed bug in nine-level tones (in PUA) feature
- Made Chinantec tones larger, added 02C9 to this feature
- Fixed bug in GSUB table to work in Pango

### 15 Dec 2006 (SIL NRSI team)  Charis SIL version 4.0.04 beta 1 (Version 4.004)
- Beta release (should not be distributed!)
- Added support for Unicode 5 Latin and Cyrillic additions
- Other new chars: 2053, 211F, 2123, 2423, FE20..FE23
- Numerous new PUA characters
- Deprecated some existing PUA chars now added to Unicode
- New features:
	- Open O alternate
	- Chinantec tones
	- Pitch contour tramlines
	- Cyrillic italic alternates
- Tone bars no longer limited to 3 sequences (OpenType)
- Added glyphs for nine-level tones (in PUA)
- Design changes to some Greek, Cyrillic, ogonek and modifier glyphs,
  particularly in italic faces

### 31 Jan 2006 (SIL NRSI team)  Charis SIL version 4.0.02 (Version 4.002)
- First version released under the SIL Open Font License

## License

This Font Software is licensed under the SIL Open Font License, Version 1.1.
This license is available with a FAQ at https://openfontlicense.org

## Repository Layout

This font repository structure is inspired by [Unified Font Repository v0.3](https://github.com/unified-font-repository/Unified-Font-Repository), modified for the Google Fonts workflow.
