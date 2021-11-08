CSV into Nested JSON which is structured to be imported into FoundryVTT.

The CSV headers are JSON fields.  Nested fields will be labeled: `data.description` or `data.stunts.name` with each nested leveling being dictated by a `.`

TODO:  
`data[row['name']] = record = {}` should provide nothing, there is no primary key at the base level  
`data.stunts.name` SHOULD be used as a primary key within the nested structure  
