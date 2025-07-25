```antlr
ESC : "\u001b";
BEL : "\u0007";
SAIOSMP_CMD : DCS "!SAIOSMP:";  // Can be changed in the future
SAIOSMP_ENDCMD : ESC "\\" /* preferred */ | BEL;
```
