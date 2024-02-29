rule "adjust first indicator of 852 for ERC materials"
when
	(exists "852.c.NF")
then 
	changeFirstIndicator "852" to "1" if (exists "852.{8,*}")
	changeFirstIndicator "852" to "1" if (exists "852.{0,*}")
end
