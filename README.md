Strings pulled out of Homeland's data files.

File format:
windows line breaks(\r\n)
Character encoding is Shift JIS
If the first character is a '#' this string will be ignored
string id, followed by line break
a list of file and offset(int hexadecimal) pairs, ending with an empty line
	there is a tab between the file and the offset, followed by a line break
The number of bytes in the String(called length) in hexadecimal, followed by a line break
The original text(there are length bytes), followed by a line break(because it looks better in a text editor).
the replacement text(length bytes), followed by a line break
Carriage return, line feed(Windows new line)

there are 23409 unique strings
