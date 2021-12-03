## Configuring Github's Personal Access Token to Make Code Pushes Easier

*Before you start reading, this is an article that will teach you how to configure Github's Personal Access Token so that you need not have to copy-paste the Token each time you push code to remote.*

## Problem and Research

Recently I faced an issue with `git push` on VS Code. 

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1637381615284/uGEeGmBQP.png)

I rechecked my VS Code terminal to see if I was still logged into git and confirmed I was.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1637382189449/sLHEHdA_0.png)

## Unsuccessful Attempts to Solve it

I immediately tried a Google search for the error `remote: no anonymous write access`. I could see that there were a few issues on VS Code's Github Repo regarding this issue.

- [Issue 1](https://github.com/microsoft/vscode/issues/137161)
- [Issue 2](https://github.com/microsoft/vscode/issues/136791)

The discussion looked like there was some issue or bug with VS Code's latest version 1.62.2 that stopped users from pushing their code in the traditional way of `git push origin branch-name`. One suggestion was to downgrade the VS Code's version to 1.62.0 and try pushing the code.

But, that did not work for me. 

## Introspection and More Research

I was aware that Github's Personal Access Tokens could be used to push changes from the terminal. It looked like a cumbersome process.

Entering my GitHub user name and PAT (Personal Access Token) as the password for each push would make the code-commit-push process much difficult. 

GitHub stopped accepting passwords through the terminal, since August 2021. 

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1637383569559/uLljHrzLz.png)

This would make it much harder for developers to push the commits to remote.

After talking with a  [mentor](https://hashnode.com/@eduardovedes) , I understood that it was not an issue with VS Code but, with the authentication during the push. 

He also said that he used the PAT to push the changes.

Now my goal was to google PAT and see if there was any way to authenticate my pushes without having to enter the Personal Access Token for each push.

## Solution

I read through GitHub Documentation, Stackoverflow and Ask Ubuntu. I also did some small trials using the PAT, to arrive at a solution. 

The gist of this solution is that each Repo I was working on had to be authenticated with the PAT so that the pushes could be done seamlessly.

### Adding the PAT to the Repositories

Generate a Personal Access Token, if you don't have one. Read  [this document](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to understand how it can be generated.

Once you have saved your PAT, it must be added to the Repos on your local machine. 

Open the VS Code Terminal from the Repo you want to add the PAT to.

Enter `git remote set-url origin https://yourPAT@github.com/yourGitUserName/yourGitRepo.git`.

*Note: It's not a double-line command. **Do not** hit enter after `origin`.*

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1637385774257/NsbsFLvg-.png)

Now you can commit and push without having to enter the Personal Access Token every time you push your commits to remote.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1637384603937/oyxoBE09o.png)

## Conclusion

This approach saves time and does not compromise security. Feel free to write to me if you have better suggestions on how this can be solved. My contact details are available on my Profile.


#2Articles1Week #Github