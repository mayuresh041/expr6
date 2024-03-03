
C:\Users\91987>ia1:
'ia1:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\91987>Desktop:
'Desktop:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\91987>desktop:
'desktop:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\91987>ia1
'ia1' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\91987>mkdir ia2

C:\Users\91987>cd ia2

C:\Users\91987\ia2>git init
Initialized empty Git repository in C:/Users/91987/ia2/.git/

C:\Users\91987\ia2>git clone https://github.com/mayuresh041/m05.git
Cloning into 'm05'...
remote: Enumerating objects: 9, done.
remote: Counting objects: 100% (9/9), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 9 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (9/9), done.

C:\Users\91987\ia2>git checkout -b fb1
Switched to a new branch 'fb1'

C:\Users\91987\ia2>cd m05

C:\Users\91987\ia2\m05>git fetch origin
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 920 bytes | 83.00 KiB/s, done.
From https://github.com/mayuresh041/m05
   8984751..d86da12  main       -> origin/main

C:\Users\91987\ia2\m05>git rebase origin/main
Successfully rebased and updated refs/heads/main.

C:\Users\91987\ia2\m05>git add .

C:\Users\91987\ia2\m05>git commit -m "hello"
[main 7205394] hello
 1 file changed, 1 insertion(+)

C:\Users\91987\ia2\m05>git fetch origin
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 924 bytes | 84.00 KiB/s, done.
From https://github.com/mayuresh041/m05
   d86da12..c7d05dd  main       -> origin/main

C:\Users\91987\ia2\m05>git rebase origin/main
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply 7205394... hello
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".
Could not apply 7205394... hello

C:\Users\91987\ia2\m05>git add .

C:\Users\91987\ia2\m05>git rebase --continuie
error: unknown option `continuie'
usage: git rebase [-i] [options] [--exec <cmd>] [--onto <newbase> | --keep-base] [<upstream> [<branch>]]
   or: git rebase [-i] [options] [--exec <cmd>] [--onto <newbase>] --root [<branch>]
   or: git rebase --continue | --abort | --skip | --edit-todo

    --[no-]onto <revision>
                          rebase onto given branch instead of upstream
    --[no-]keep-base      use the merge-base of upstream and branch as the current base
    --no-verify           allow pre-rebase hook to run
    --verify              opposite of --no-verify
    -q, --[no-]quiet      be quiet. implies --no-stat
    -v, --[no-]verbose    display a diffstat of what changed upstream
    -n, --no-stat         do not show diffstat of what changed upstream
    --stat                opposite of --no-stat
    --[no-]signoff        add a Signed-off-by trailer to each commit
    --[no-]committer-date-is-author-date
                          make committer date match author date
    --[no-]reset-author-date
                          ignore author date and use current date
    -C <n>                passed to 'git apply'
    --[no-]ignore-whitespace
                          ignore changes in whitespace
    --[no-]whitespace <action>
                          passed to 'git apply'
    -f, --[no-]force-rebase
                          cherry-pick all commits, even if unchanged
    --no-ff               cherry-pick all commits, even if unchanged
    --ff                  opposite of --no-ff
    --continue            continue
    --skip                skip current patch and continue
    --abort               abort and check out the original branch
    --quit                abort but keep HEAD where it is
    --edit-todo           edit the todo list during an interactive rebase
    --show-current-patch  show the patch file being applied or merged
    --apply               use apply strategies to rebase
    -m, --merge           use merging strategies to rebase
    -i, --interactive     let the user edit the list of commits to rebase
    --[no-]rerere-autoupdate
                          update the index with reused conflict resolution if possible
    --empty (drop|keep|ask)
                          how to handle commits that become empty
    --[no-]autosquash     move commits that begin with squash!/fixup! under -i
    --[no-]update-refs    update branches that point to commits that are being rebased
    -S, --[no-]gpg-sign[=<key-id>]
                          GPG-sign commits
    --[no-]autostash      automatically stash/stash pop before and after
    -x, --[no-]exec <exec>
                          add exec lines after each commit of the editable list
    -r, --[no-]rebase-merges[=<mode>]
                          try to rebase merges instead of skipping them
    --[no-]fork-point     use 'merge-base --fork-point' to refine upstream
    -s, --[no-]strategy <strategy>
                          use the given merge strategy
    -X, --[no-]strategy-option <option>
                          pass the argument through to the merge strategy
    --[no-]root           rebase all reachable commits up to the root(s)
    --[no-]reschedule-failed-exec
                          automatically re-schedule any `exec` that fails
    --[no-]reapply-cherry-picks
                          apply all changes, even those already present upstream


C:\Users\91987\ia2\m05>git rebase --continue
[detached HEAD 8fdad5a] savehello
 1 file changed, 3 insertions(+)
Successfully rebased and updated refs/heads/main.

C:\Users\91987\ia2\m05>git push origin fb1
error: src refspec fb1 does not match any
error: failed to push some refs to 'https://github.com/mayuresh041/m05.git'

C:\Users\91987\ia2\m05>git push origin main
fatal: User cancelled dialog.
Username for 'https://github.com': mayuresh041
Password for 'https://mayuresh041@github.com':
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 281 bytes | 281.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/mayuresh041/m05.git
   c7d05dd..8fdad5a  main -> main
# expr6
