Add comma at start
---
FindWhat : ^              // regex to start at each line
Replace  : '              // replace start of line/s with quote to create JSON

Add comma at end
---
FindWhat : $              // regex to end of line
Replace  : ',             // replace end of line/s with quote+comma to create JSON

Delete text after comma
---
FindWhat : ,(.*)              // regex any text after comman
Replace  :   ',               // replace all commas with quote+comma use it to create JSON


Delete Line
---
FindWhat : (?-s)^.*0000000001243730|0000000001243731|0000000001243732.*\R
Replace: empty

Trim Trailing Space 
---
\s+$

Trim Leading Space
---
^\s+

