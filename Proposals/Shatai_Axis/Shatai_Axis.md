# Proposal Summary Form: Shatai Axis

## Administrative Information
**Proposers name:** Myles C. Maxfield, Apple Inc, and Koji Ishii, Google Inc.

**Proposal name:** Shatai_Axis

**Date of submission:** 3-26-19

**New or revised proposal:** New

**Previous revision date:** N/A

## General Technical Information
**Overview:** A variation axis to control the degree of shatai slant in vertical Japanese text.

**Related axes:** N/A

**Similar axes:** 'slnt', 'ital'

**Axis type:** Optical

## Proposed Axis Details

**Tag:** shti

**Name:** Shatai

**Description:** This axis controls the skew angle of vertical Japanese text. When drawn with shatai,
vertical japanese text should be skewed such that the logical top of the line (physical right) is pulled
toward the logical beginning of the line (physical top). This is opposite from the direction Latin text is
skewed. In addition, Vertical Japanese text uses upright characters in accordance with UAX #50, which
means 'slnt' is not applicable.

**Valid numeric range:** -90 - 90

**Scale interpretation:** This is the skew angle in degrees. Positive values act according to the behavior
described in the Description above.

**Recommended or required &ldquo;Regular&rdquo; value:** 0

**Suggested programmatic interactions:** When rendering and laying out vertical italicized text, a program
may set this value to some common value, such as 14.

**UI recommendations:** This axis should be used when drawing vertical italicized text. If this axis is not
present in the font, the program may choose to implement this effect by applying a mathematical skew to
the characters.

**Script or language considerations:** This is mainly applicable to Japanese, but is useful in all scripts
that are written vertically and have the concept of italics.

**Additional information:** The logical height (physical width) of the characters should not be altered;
this is a skew, not a rotation.

## Justification
**Vendor commitments:** WebKit, Chrome

**Conventionality benefits:** Providing an alternative to a mathematical skew would increase the
typographic quality of the text being rendered. Allowing artists to fine-tune the skew would produce
higher quality renderings.

**Interoperability benefits:** Beautiful vertical italics will be ubiquitious.

## Other Supporting Information

[Example](https://partnerhelp.netflixstudios.com/hc/en-us/article_attachments/204555817/ja_tt3.png),
[Example](https://plaza.rakuten.co.jp/picardy3rd/diary/200705070000/).
