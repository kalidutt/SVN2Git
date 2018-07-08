# SVN2Git



tfsqatest@VM-QATest-02 MINGW64 ~/Desktop/meme
$  git init --bare /c/Users/tfsqatest/Desktop/meme/gitrepo/


tfsqatest@VM-QATest-02 MINGW64 ~/Desktop/meme
$ svn log -q | awk -F '|' '/^r/ {sub("^ ", "", $2); sub(" $", "", $2); print $2" = "$2" <"$2">"}' | sort -u > authors.txt

tfsqatest@VM-QATest-02 MINGW64 ~/Desktop/meme
$ svn log --stop-on-copy http://iris-svn-01.irissoftware.com:8080/svn/Devops-GitHubRepo


