
# Markdown from git

Git repositories contain a lot of markdown files. We all know about the famous
README in the root of repositories. But there is a lot of other documentation
hidden in git repositories ready to be shared with the world. 

One example is [adr][3], architectural decision records. These records are often 
maintained by developers in git repository. Wouldn't it be nice if you can
share them in Confluence?

Another example is _docs as code_. Write your documentation in markdown and
process with an engine such as [Jekyll][4] and you are ready to go. Now you can easily
share specific parts of your documentation in Confluence as well!

## Up to date documentation

If you update markdown files in Git, you no longer have to worry about going
to Confluence to update the same thing there. Just stick to Git and 
[Git for Confluence][1] will update the content in... well... Confluence.

## Safe sharing

Securely share Git files with Confluence users who don't have access to the Git 
repository. Connect your Git provider with Confluence and share content on your 
behalf based on a safe OAuth flow.

[1]: https://marketplace.atlassian.com/apps/1211675/git-for-confluence
[2]: https://avisi-apps.gitbook.io/git-for-confluence-cloud/
[3]: https://adr.github.io/
[4]: https://jekyllrb.com/
