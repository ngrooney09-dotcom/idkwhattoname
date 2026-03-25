This is a user documentation for Git Hub. It demonstrates creating a new repository, pushing existing code to your repository,
connecting git bash to your VS code terminal. The following demonstrates potential errors you may encounter.

WHAT’S HAPPENING?

If you see errors like:

error: You have not concluded your merge (MERGE_HEAD exists)

or

error: Merging is not possible because you have unmerged files

It means Git started a merge, but you haven’t finished resolving conflicts yet.

You might also see:
(main|MERGING)

That means you are currently in the middle of a merge.

STEP-BY-STEP FIX

CHECK STATUS

Run:
git status

This shows:

Which files have conflicts
What Git expects you to do next
FIND CONFLICTED FILES

Look for:
both modified: filename

These files need to be fixed.

OPEN AND RESOLVE CONFLICTS

Inside the file, you’ll see:

<<<<<<< HEAD
your code

incoming code

branch-name

Meaning:

HEAD = your version
Bottom section = incoming changes
FIX THE FILE

Edit the file and choose what to keep.

Example:

Before:
<<<<<<< HEAD
console.log("My version");

console.log("Their version");

branch-name

After:
console.log("Final version");

IMPORTANT:
Remove ALL of these lines:
<<<<<<<
MARK AS RESOLVED

Run:
git add .

Or per file:
git add filename

FINISH THE MERGE

Run:
git commit

Save and close the message — merge complete.

ABORT THE MERGE (OPTIONAL)

If you want to cancel everything:

git merge --abort

Then retry:
git pull

BACKUP FIX (IF NEEDED)

git reset --merge

QUICK WORKFLOW

git status

fix conflicts

git add .
git commit

TIPS

Always run git status if unsure
Never leave conflict markers in files
Git won’t decide for you — you must choose
