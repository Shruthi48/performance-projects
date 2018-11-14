# performance-projects

Git commands

- [ ]  git add 
- [ ] git commit
- [ ] git push    or git push —upstream-set issue/lego-2730

- [ ] gcm
- [ ] gf
- [ ] gm
- [ ] gst
- [ ] gco -
- [ ] grbm
- [ ] git push force-with-lease


Squash

- [ ] glol
- [ ] grb origin/master
- [ ] grbi origin/master
- [ ] gst
- [ ] gp -f

changing rebase release

git rebase --onto release/v3.13.0 f05c8b805d03faa95e9c31cf6ce49f8b1e583377^

git branch -a | grep v3.13.0

git rebase -i --onto remotes/origin/release/v3.13.0  82049a42fe4d5f60fe8c3f3113616e7751ff6e7a^

If you rebase it onto master first then...

git rebase --onto=master 17df13ba5b9ee9bf3a4b7252bf51f1fee04bc522^

Then squash the commits after;

git rebase -i HEAD^^^

[3:16] 
... and see how that goes?

cherry-pick 
git cherry-pick <commit-hash>

git rev-parse HEAD

squash commits 
git rebase -i head~5 



Remove package.lock
git checkout develop -- package-lock.json
gc --fixup cdc2d20
git config --global rebase.autosquash true
grbi cdc2d20~
gp -f --no-verify



copy one branch to another
git checkout -b feature/lego-8092-integrate-2
git push origin feature/lego-8092-integrate-2
