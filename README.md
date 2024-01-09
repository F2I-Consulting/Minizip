
# Minizip 1.1
 - This is a copy of the official zlib 1.3 "contrib/minizip" folder without test, demo and extra files.
 - You can find binary versions for windows in the Release tab. If you don't find the version for your windows environment, please just ask for it (create an issue).
 - You can build the library quite easily by your own by using the cmake file.
 - The license is defined in MiniZip64_info.txt file.

## RHEL 
Our RHEL 6 machines have zlib.h version 1.2.3 so zip.c will not compile because the type z_crc_t is undefined. An easy fix, since I don't think you care about encrypting RESQML packages, is to simply compile on Linux with -DNOCRYPT.
RHEL 7 seems to have zlib.h version 1.2.7 which does have the z_crc_t type however. (See issue #2)
