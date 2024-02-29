rule "call number move"
when
	TRUE
then
	changeSubField "852.h" to "x"
	changeSubField "852.i" to "x"
end 