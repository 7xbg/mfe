# mfe
Meth Fueled Energy is a program with a really simple command handler.
I dunno why I made this but I did so yaa.
*(I kinda just made this to test memory editing)*

# mfe help
**Commands**:
 - log
   - usage: log [message] [r g b] [bold(true / false)]
   - example: log [hello world] [255 0 0] [true]
   - note: [ and ] are seperators for varibales use them
 - logline
   - usage: logline [message] [r g b] [bold(true / false)]
   - example: logline [hello world] [255 0 0] [true]
   - note: [ and ] are seperators for varibales use them
     - p.s: its the same as log but it adds a new line
 - msgbox (messagebox)
   - usage: msgbox [message] [title]
   - example: msgbox [hello world] [welcome]
 - op (open process) **PRETTY MUCH USELESS RN**
   - op: [process name]
   - example: op [ac_client.exe]
 - rpm (read process memory)
   - usage (pointer): rpm [base,offset1,offset2...] [type] [process name]
   - example (pointer): rpm [509B74,F8] [int] [ac_client.exe] *(reads health in AssaultCube version 12.0.2)*
   - note: This is a work in progress so it can only read integers *(4 byte)*
 - wpm (write process memory)
   - usage (pointer): wpm [base,offset1,offset2...] [type] [process name] [value]
   - example (pointer): wpm [509B74,F8] [int] [ac_client.exe] [1000] *(sets health to 1000 in AssaultCube version 12.0.2)*
   - note: To NOP something, replace [address] with the address and replace [value] with 90 for each byte
