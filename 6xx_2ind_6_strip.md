rule "remove subject headings with second indicator 6"
when
	(TRUE)
then
	removeField "6**" if (exists "6**.{*,6}")
end