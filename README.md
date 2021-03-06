# LiveCode.plist


**Attribution:** 2014-11-25: History: This plist was adapted from the LiveScript.plist (a completely different language use as a kind of "IDE" for Javascript) by Ben Rubinstein. Brahmanathaswami added some folding features. He also set this up as a separate public repository.

**USAGE** 

Put the LiveCode.plist into  /Application Support/BBEdit/Language Modules. Restart BBEdit.

**CAVEATS** 

1. This is working on Brahmanathaswami's machine running BBedit 11 under Yosemite, but it is not working on some other stations with Mavericks and an earlier versions of BBEdit. I am out of my depth on solving that problem.
2. The Language Features key section at the bottom "Open Statements Block" has been added for commands and functions which will fold properly, but IF and Switch  do not fold. It also fails if you try to add this "Open Statements Block" to to the existing Language Features key above. Theoretically it makes more sense to be part of that key. Disclaimer. I have no idea what I'm doing and just going on grit and intuition. So this could be buggy. 
3. Note that when folding a node the "end ###" part of the command disappears also into the fold. It would be nice to fix this so that we are not having the anxiety that the fold was "greedy" and collapsed more than it should. Ideally we could see

on myCommand

 ...... # many folded statements here
 
end myCommand
