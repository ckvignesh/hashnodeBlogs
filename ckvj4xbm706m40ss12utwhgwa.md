## Github Submodules and how you can use them for your Projects

## Introduction

Before we get into the crux of Github submodules, let me give you some context. I'm writing this article on Day 9th of my #100DaysofCode challenge. I'm working my way through freeCodeCamp's Fronted certifications and building a portfolio website on the side. I also participated in the #Hacktoberfest, last month.

I document my progress in freeCodeCamp by saving the important answers in [this repositary](https://github.com/ckvignesh/FreeCodeCamp). But, I faced a challenge while updating my progress in the [#100DaysofCode log file Repo](https://github.com/ckvignesh/100-days-of-code/).

It was cumbersome to handle both these Repos as they needed to be updated daily, to keep track of my progress. Then I created a lot of other Repos too, to document solutions to smaller problems that I solved. Mostly in CSS games as I was learning CSS in freeCodeCamp back then. 

I also needed to find a way to map these Repos into my #100DaysofCode log Repo as proof. You could say that I can easily add the link of those Repos to my Markdown log file. But, I felt that would become a daily chore as I keep increasing the number of folders for each section or topic.

Yesterday, I moved a few of these Repos to my #100DaysofCode Repo and tried to commit it. But, the terminal threw this message.

![Error.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1635917783549/ST4vwlwkp.png)

This is how I stumbled upon GitHub submodules.

## Github Submodules

When you're working on a project, you may have to use another project within it. In my case, I owned all the Repos I used. But, it need not be like that always. You may sometimes be using a 3rd party's Repo for your work. Sometimes, one Repo may be needed for many Projects. In any of these cases, you will have to rely on Github Submodules.

Git submodules allow you to Repo as a subdirectory or a folder within another Repo. Let's now see how we can add Submodules without making such an error as I made before.

The usual command to clone a repo is like this:

`git clone https://github.com/uName/repoName.git`

But this won't make it a submodule. It'll remain as a standalone Repository. Now, this is not how we add a Submodule in another Repository. The command to clone it is:

`git submodule add https://github.com/uName/repoName.git` 

Once this has been completed successfully, try running `git status` to see what are the new files added. You'll see this.

![Gitmodules.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1635918611200/MVvc9Jhz_.png)

You can see 2 things here, one the submodule Repo and then a file named `.gitmodules`. It's similar to the .git folder that's hidden and you may not see it unless you enable "show hidden files". 

Let's check `.gitmodules`.

![Submodule file.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1635918830255/yZgNk8YLZ.png)

Here, you can see the details of the submodule. This is the file that tells Git about your submodule. Now you can work on your Repo or the submodule Repo and commit it to Github.

This is how my submodules appear in the Parent Repo.

![Submodules.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1635919068274/hJb372Bs-y.png)

It lets you click the folders and leads you to the submodule Repos directly. The ` @ xyz123 ` value after the submodule Repos show the last commit of the submodule/child Repo that's present in the Parent Repo's submodule.

## Working on Submodules and keeping them updated within the Parent Repository

Now let me make some changes to both these submodule/child Repos and commit them. But this won't change the ` @ xyz123 ` values with the folder names in the Parent Repo. They'll remain constant like this:

![Submodules.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1635919068274/hJb372Bs-y.png)

Now, if you need the updated version of the child Repo within your Parent Repo, you must add these changes from the root of the parent Repo. It'll show up like this:

![1.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1635919888275/nN56FRCuQ.png)

Once you commit and push the changes, the changes are reflected in the Parent Repo. You can see the difference in the commit numbers in this picture.

![2.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1635919935896/9GwJmp8et.png)


## Conclusion

Github Submodules are a very vast topic and this article is just to help you get started with it. There is a lot more to explore here.

You can read more from the official documentation, [here](https://git-scm.com/book/en/v2/Git-Tools-Submodules).





#github #100DaysOfCode #Submodules #git #2Articles1Week