# Github Remote Permission Denied

Try to upload a repo on github and go through all the steps upto:

`git push -u origin master`

At that point it gives the following error:
```
remote: Permission to [***/***.git] denied to [***].
fatal: unable to access 'https://github.com/***/***.git/': The requested URL returned error: 403
```
I think the issue is that you were logged into another Git account before `user1` and now you are trying to push to `user2`.

Unable to access https means: this has nothing to do with SSH 
(and switching to SSH, while possible, does not explain the original issue)

This has to do with credential caching, meaning Git will by default provide the credentials 
(GitHub account and password) of the old account while you are trying to push to the new account.

See if you have a [credential helper](https://git-scm.com/book/en/v2/Git-Tools-Credential-Storage) 
that would have cached your (old account) credentials (username/password) used to authenticate you.

`git config credential.helper`

On Mac, just goto/open your `Keychain Access` -> search for `github.com` related file -> and edit `credentials` there.

On Windows, for example, that would be the `Windows Credential Managers`.
Open the Windows Credential Store, and see if the first user is registered there: 
delete that entry, and you will be able to authenticate with the second user.
