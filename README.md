# WarbleCustomWordList
Warble is a Linux version of Wordle.  Or maybe Wordle is a version of Warble.  I don't know.  In either case, this set of apps lets you customize your Warble word list.  So far, it only works on recent versions of Ubuntu where Warble is distributed as a Snap.

This comes with a set of words from Hermit Dave.  If you want to use a different list, give the file a unique name and save it in the folder with the rest of these files.  It needs to be a plain text file whose name ends in ".txt", but beyond that there aren't really any limitations.  For exanmple, the Hermit Dave list contains usage counts.  We filter out everything except words with five letters, so those counts will get filtered out.

Run Make_5LetterWords to make 5letterwords.txt

* If you have a custom list, pass the filename without the ".txt" like "Make_5LetterWords MyList"
* Make_5LetterWords will take the list and turn it into 5letterwords.txt.  It will make sure all the words in the list are in Warble's dictionary so you don't end up with an unsolvable puzzle.

Run UpdateWarbleWordList
  
* This will take 5letterwords.txt and make it your Warble word list.  You probably don't want Warble to be running when you do this.

Enjoy!


PS:  
* I included a snapshot of the Warble source code so you'd be sure to have a dictionary.txt file to work with.  If you want, you can go to https://github.com/avojak/warble, get the latest code, and replace what's here.
* The HermitDave_Source.html file will take you to Hermit Dave's web site.  I started with his 50,000 list then trimmed it down to 40,000 to get rid of more obscure words.  There are still a bunch here, but you can edit WordsToIgnore.txt then run the two commands to get rid of ones you don't want to see (again).
