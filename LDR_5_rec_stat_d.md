rule "set rec stat to d"
when
	(TRUE)
then
	replaceControlContents "LDR.{5,1}" with "d"
end