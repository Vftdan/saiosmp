```antlr
// All hex escapes in [\u0080-\u00FF] are in the LATIN-1 / ISO 8859-1 encoding
ESC : "\u001b";
BEL : "\u0007";
C1ST : "\u009C";
DCS : ESC "P";
SAIOSMP_CMD : DCS "!SAIOSMP:";  // Can be changed in the future
SAIOSMP_ENDCMD : ESC "\\" /* preferred */ | BEL | C1ST /* don't */;
```
