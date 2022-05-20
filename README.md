# Github


In addition to the answers above, the following worked for me : -

Scenario -

I pushed my_branch to origin successfully.
I made few more changes.
When I tried to push again, (after doing add, commit of course), I got the above mentioned error.

Solution -

Always check this file before push code in repo
vi .git/config
to find out the branch head


 1. git checkout **my_branch**
 2. git add, commit your changes.
 3. git pull origin **my_branch** (not origin, master, or develop)
 4. git push origin **my_branch**
