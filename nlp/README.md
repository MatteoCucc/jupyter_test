requirements for the scripts

(how to update pip:   
*pip install --upgrade pip*)

#### How to install gensim

open terminal and run:    
*pip install gensim*   
or   
*pip install --upgrade gensim*

#### How to install nltk
*pip install nltk*


#### How to install stop-words
*pip install stop-words*

#### How to install TreeTagger
Follow the instructions at http://www.cis.uni-muenchen.de/~schmid/tools/TreeTagger/:   

1. Download the tagger package for your system:    
http://www.cis.uni-muenchen.de/~schmid/tools/TreeTagger/data/tree-tagger-linux-3.2.1.tar.gz
2. Download the tagging scripts into the same directory:   
http://www.cis.uni-muenchen.de/~schmid/tools/TreeTagger/data/tagger-scripts.tar.gz
3. Download the installation script install-tagger.sh:    
http://www.cis.uni-muenchen.de/~schmid/tools/TreeTagger/data/install-tagger.sh
4. Download the parameter files for the languages you want to process:    
http://www.cis.uni-muenchen.de/~schmid/tools/TreeTagger/#parfiles    
(for italian: http://www.cis.uni-muenchen.de/~schmid/tools/TreeTagger/data/italian-par-linux-3.2-utf8.bin.gz)
5. Open a terminal window and run the installation script in the directory where you have downloaded the files:   
*sh install-tagger.sh*
6. Make a test, e.g. *echo 'Salutando il mondo!' | cmd/tree-tagger-italian* 

After the step below, open file .profile and set PATH so it includes user's private bin directories:    
      
PATH="$HOME/bin:$HOME/.local/bin:$PATH"
PATH="$PATH:/home/ubuntu/pathto/treetagger/cmd:/home/ubuntu/pathto/treetagger/bin"
