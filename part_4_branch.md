<h2> Git Branching </h2>

A chain of linearly connected commits is called a <b> branch </b> typicaly the first and main branch in a repository will be known as the 'master' branch. This is often kept as a clean working copy of your code. Repositories can have multiple branches that divere from each other however. Each branch can contain a different version of the working files, and as long as these changes have been commited the user can swap between different branches.

This is most often used to create 'feature branches', where a specific feature, addition, or bug fix can be worked on without affecting the clean working copy of the master branch. When a feature is complete it can be <b> merged </b> back into the master branch (or any other branch) to update the master branch to a new working version. This can also be nested, so branches can have branches infinititum. There can also be multiple branches open for one branch at a time.

If you try to merge a branch into another but that branch has had changes since the orignal branch was split from it which contradict with the new changes you are trying to merge, this results in a <b> merge conflict </b>. In the case of a merge conflict, it requires the user to manually review the two sets of changes and selectively choose which to keep. This can result in a lot of complications, so it is still best to try and avoid working on the same bit of code twice.

To list all current branches:

    git branch
  
    git branch new_feature_branch
  
    git checkout new_feature_branch
  
  
