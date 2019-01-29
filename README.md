## Git Remote

/home/dq/chatbot$ git diff  

## Switch to specific commit #
/home/dq/chatbot$ git reset --hard $HASH 

HEAD is now at e7fc4dd Updated README.md

## Pull from Remote Repo #
/home/dq/chatbot$ git pull origin master 

From /dataquest/user/git/chatbot                                                
 * branch            master     -> FETCH_HEAD                                   
Already up-to-date.  

## Referring to the most recent commit #
/home/dq/chatbot$ git reset --hard HEAD~1

HEAD is now at 5ea52d4 Add the initial version of README.md 

## Pull from Remote Repo #
/home/dq/chatbot$ git pull origin master 

From /dataquest/user/git/chatbot                                                
 * branch            master     -> FETCH_HEAD                                   
Updating 5ea52d4..e7fc4dd                                                       
Fast-forward                                                                    
 README.md | 2 +-                                                               
 1 file changed, 1 insertion(+), 1 deletion(-)                                  

#To review, git reset is a powerful command that is used to undo local changes to the state of a Git repo. Git reset operates on "The Three Trees of Git". These trees are the Commit History ( HEAD ), the Staging Index, and the Working Directory. ... The options --soft, --mixed , and --hard can be passed to git reset .
