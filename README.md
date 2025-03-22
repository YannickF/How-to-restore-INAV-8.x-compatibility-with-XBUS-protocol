Replace files (in rx folder) and compile for your flight controler (instuctions for compiling are available on iNav documentation)

MULTIPLEX MLINK receiver can send a serial message to flight controler. The protocol used is SRXL V1 or SRXL V2 which is specific to Multiplex MLINK receiver.
This protocol is no longer decoded by iNav.

As it's very similar to SUMD protocol (used by Graupner) it was very easy to modify the source code to decode SRXL messages instead of SUMD messages.

Please note that you will not be able anymore to decode a true SUMD protocol.



By the way, when I compiled the project from source code 8.0.1, the version indicated by Flight Controler was 9.0.0 instead of 8.0.1

Modify information about version in CmakeLists.txt in cmake folder

Search for a line similar to :

project(INAV VERSION 8.0.1)


