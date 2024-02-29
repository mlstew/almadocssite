rule "add note to existing 876 regarding withdrawal"
priority 1
when
not exists "876.x.Withdrawn_2024"
then
addSubField "876.x.Withdrawn_2024"
end

rule "Add field 876"
priority 2
when
not exists "876"
then
addField "876.{-,-}.x.Withdrawn_2024"
end