# learn-git

## Basic workflow

If you want to develop a new feature. I would recommend you the following working steps:

First of all ```pull``` the code from the remote repository. Just to be sure, that you work on the most recent code-base.
you should ```pull``` from the ```main``` branch. The ```main``` branch, should normally contain the most recent and
*TESTED* code. Keep in mind, that if you use ```pull```, it directly changes your local code. If you first want to peek 
what changes where applied, use the ```fetch``` command.

(pull vs. fetch)[https://www.git-tower.com/learn/git/faq/difference-between-git-fetch-git-pull/]

Now, since you have the most recent code, you should checkout a branch.
If you use the command below, you will create a new branch, and you automatically switch your context to this branch.

```git checkout -b <new branch> ```

replace <new branch> with a *meaningful* branch-name. No-one knows what you are doing on a branch called "fancy-feature".
(branch-naming)[https://stackoverflow.com/questions/273695/what-are-some-examples-of-commonly-used-practices-for-naming-git-branches]

Now it is time to do some actual work. Implement you feature. As you do so, try to commit the changes in useful steps.
That means git is a version control system, use it! Don't commit after every character you added, but the smaller 
the commits, the better the work process can be traced and possibly reset to a certain position.

If you have to add a new file for your feature use:

```git add <filename>```

No matter if you added a new file, or editing an existing one, after your work is done, you have to commit it.
You do so with:

```git commit -m "feat: add fancy new button"```

(How to commit)[https://www.conventionalcommits.org/en/v1.0.0-beta.2/]

Now, your work is done, what happens now? Of course want our new feature being part of the actual code-base which is 
based in the ```main``` branch. but we do remember, that the main branch only contains tested, working code. Of course,
you are able to verify this by yourself, but if you are working on a bigger project, it can be quickly overwhelming 
for one person to 
have everything in mind. Since you are working with a Team of Developers here, we should use something like a review 
process. GIT already took care of this situation. We are now leaving the command line interface and focus on the 
repository in our browser. 

TODO: Picture.

Where your find this feature is depending on the platform your are using github/gitlab/git-whatever 
but all those platforms offering the merge/pull-request feature. This is a review process.
Here you want to MERGE your new feature branch into the ```main``` branch. For this purpose it makes sense, 
that you ask your developer colleagues to review your code. Do not take it personal, 
this is NOT a finger-pointing process, it is a quality process.  
If all contributors are fine with the code quality it can get merged into the ```main``` branch. 
A new version of your code-base is born. 
If you want to add another new feature to your code, start reading this again. 
(Or maybe just do it, since you already now the Steps now)



