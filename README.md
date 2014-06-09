Strings pulled out of Homeland's data files.

Extracted Strings File format
-----------------------------
unix line breaks(\n), Homeland uses the same
Character encoding is Shift JIS
If the first character is a '#' this string will be ignored
String id, followed by line break
A list of file and offset(int hexadecimal) pairs, ending with an empty line
	There is a tab between the file and the offset, followed by a line break
The number of bytes in the String(called length) in hexadecimal, followed by a line break
The original text(there are length bytes), followed by a line break(because it looks better in a text editor).
Carriage return, line feed(Windows new line)

Replacement Strings File Format
-------------------------------
unix line breaks(\n), Homeland uses the same
Character encoding is Shift JIS
If the first character is a '#' this string will be ignored
Id of the String to replace, followed by line break
replacement String bytes, with a '|' indicating where it ends(So don't use one in the replacement string itself), then a line break.
If the replacement string is longer than the original, the patcher will give an error.
The patcher will handle replacement strings that are shorter than the orginal.

there are 23660 unique strings

If a string looks weird, hl-string-ef9df550for example, create an issue.