# What is a Barcode?

A barcode is basically a way of writing numbers or data in a pattern of lines and spaces that machines can quickly read.

Think of it as a visual Morse code: black bars and white gaps replace the dots and dashes. Each arrangement of thick and thin bars corresponds to digits, letters, or even whole strings of data.

[barcode image](../hardware/images/barcode.png)

## Structure

- Bars (Black lines)
- Spaces (White lines)

## Types of Barcode

- 1D barcodes (like the UPC on groceries): just a series of vertical lines.
- 2D barcodes (like QR codes): grids of squares that can hold much more data.

## Purpose:

They’re used to encode data in a compact, cheap, and scannable way. That’s why they show up in supermarkets, warehouses, tickets, ID cards, and even hospital wristbands.

🏷️ Major Types of 1D Barcodes
- UPC (Universal Product Code)<br>Used mostly in the U.S. for retail (groceries, books, etc.).<br>Variants: UPC-A (12 digits), UPC-E (compressed version).<br>Start/Stop: 101 at start, 101 at end.
- EAN (European Article Number)<br>International retail version of UPC.
- EAN-13 (13 digits), EAN-8 (short codes for small packages).<br>Similar start/stop patterns as UPC.
- Code 39<br>Early, widely used in logistics, defense, and automotive.<br>Encodes numbers, letters, and some symbols.<br>Start/Stop: represented by the asterisk *.
- Code 128<br>Very dense; can store alphanumeric + control characters.<br>Used in shipping, warehouses, and logistics labels.<br>Has special start codes (A, B, C) depending on which character set you use.
- Interleaved 2 of 5 (ITF)<br>Packs digits efficiently by encoding them across pairs of bars and spaces.<br>Common on cartons (outer shipping boxes).<br>Framed by a start and stop pattern, not identical to UPC.
- Codabar<br>Simple, older system (medical, libraries, blood banks).<br>Start/Stop: any of the characters A, B, C, or D.
- MSI / Plessey<br>Numeric-only symbology, used for inventory and shelf tags.<br>Uses variable check digits.<br>Others (less common now)
- Code 11, Pharmacode, Telepen, etc.—niche uses.

## Here we are discussing about UPC-A

There will be total of 95 lines where 7 lines indicates a digit.<br>
  start (3) + 6 digits (42) + middle (5) + 6 digits (42) + end (3). This is the structre of the UPC-A barcode.

The start and the end pattern is fixed for all the barcodes and that is 101 Black-White-Black (1-Black and 0-White)<br>
The middle patterne is alos fixed i.e.. 01010 (White-Black-White-Black-White)<br>
the left 6-digits and right 6-digits is where all the data is stored
- The first digit indicates the number system.
- The 5 digits of left side indicates the manufacturer code.
- The 5-digits of right side indicates the product code.
- The 12th digit is a check digit calculated from previos 11 digits.
