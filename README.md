## Git Remote, --hard, HEAD, reset, Remote, $HASH

/home/dq/chatbot$ git diff  

#Switch to specific commit 

/home/dq/chatbot$ git reset --hard $HASH 

HEAD is now at e7fc4dd Updated README.md

#Pull from Remote Repo 

/home/dq/chatbot$ git pull origin master 

From /dataquest/user/git/chatbot                                                
 * branch            master     -> FETCH_HEAD                                   
Already up-to-date.  

#Referring to the most recent commit#

/home/dq/chatbot$ git reset --hard HEAD~1

HEAD is now at 5ea52d4 Add the initial version of README.md 

//Pull from Remote Repo#

/home/dq/chatbot$ git pull origin master 

From /dataquest/user/git/chatbot                                                
 * branch            master     -> FETCH_HEAD                                   
Updating 5ea52d4..e7fc4dd                                                       
Fast-forward                                                                    
 README.md | 2 +-                                                               
 1 file changed, 1 insertion(+), 1 deletion(-)                                  

#To review, git reset is a powerful command that is used to undo local changes to the state of a Git repo. Git reset operates on "The Three Trees of Git". These trees are the Commit History ( HEAD ), the Staging Index, and the Working Directory. ... The options --soft, --mixed , and --hard can be passed to git reset .

#About Git HEAD variable - Git maintains a reference variable called HEAD. And we call this variable a pointer, because its purpose is to reference, or point to, a specific commit in the repository. As we make new commits the pointer is going to change or move to point to a new commit. HEAD always points to the tip of the current branch in our repository. Now, this has to do with our repository, not our staging index, or our working directory.

Another way to think of it is the last state of our repository or what was last checked out, and because it's where the repository left off or the last state, you can also say that the HEAD points to the parent of the next commit or it's where commit writing is going to take place.

I think a good metaphor to think about this is the playback and record head on a cassette tape recorder. As we start recording audio, the tape moves past the head, and it records onto it. when we press Stop the place where that record head is stopped is the place it'll start recording again when we press Record a second time. Now we can move around, we can move the head to different places, but wherever the head is positioned when we hit Record again that's where it's going to start recording.

The HEAD pointer in Git is very similar, it points at the place where we're going to start recording next. It's the place where we left off in our repository for the things that we've committed.

