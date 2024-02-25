# WarbleCustomWordList
Warble is a Linux version of Wordle.  Or maybe Wordle is a version of Warble.  I don't know.  In either case, this set of apps lets you customize your Warble word list.  So far, it only works on recent versions of Ubuntu where Warble is distributed as a Snap.

This comes with a set of words from Hermit Dave.  If you want to use a different list, give the file a unique name and save it in the folder with the rest of these files.  It needs to be a plain text file whose name ends in ".txt", but beyond that there aren't really any limitations.  For exanmple, the Hermit Dave list contains usage counts.  We filter out everything except words with five letters, so those counts will get filtered out.

Run Make_5LetterWords to make 5letterwords.txt

* If you have a custom list, pass the filename without the ".txt" like "Make_5LetterWords MyList"

Run UpdateWarbleWordList
  
* This will take 5letterwords.txt and make it your Warble word list.  You probably don't want Warble to be running when you do this.

Enjoy!
