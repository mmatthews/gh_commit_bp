# Git Commit Message Best Practices 
```
Tag: Message (Feature)[Action #123]
```

## Tag
- `Fix` - for a bug fix.
- `Update` - for a backwards-compatible enhancement.
- `Breaking` - for a backwards-incompatible enhancement.
- `Docs` - changes to documentation only.
- `Build` - changes to build process only. (ug-profile, drush etc.)
- `New` - implemented a new feature.
- `Upgrade` - for a dependency upgrade.

## Message
The **Message** is a short description of what has been done.  

The message summary should be a one-sentence description of the change. The issue or number should be mentioned at the end. If the commit doesn’t completely fix the issue, then use [refs #1234] instead of [fixes #1234]. Keep it simple and don't repeat information that is already part of the issue tracker. Avoid *"How to reproduce."*

## Action
The **Action** - depends on used task tracking, but in general case:

- `refs` "Refers to" - connecting the commit with a task or issue.
- `fixes` Closes task or issue, moving it to testing state. ***Important: use fixes only in Pull Requests***

## Feature
The **Feature** links the commit to a specific feature in our UG Drupal Platform. This is required only if the commit has an effect on a Feature. 

Here are some good commit message summary examples:

- Build: Update Travis to only test Node 0.10 (PG4)[refs #734] 
- Fix: Semi rule incorrectly flagging extra semicolon (NB3)[fixes #840] 
- Upgrade: Esprima to 1.2, switch to using Esprima comment attachment (PP1)[fixes #730]


## Formatting Suggestions

- Keep long messages to 72 columns
- Keep summary messages to 50 characters or less
- Capitalize the subject line (short message)
- Don't use periods

### Use the imperative mood in the subject line
Imperative mood just means "spoken or written as if giving a command or instruction". A few examples:

- Clean your room
- Close the door
- Take out the trash

**A properly formed git commit subject line should always be able to complete the following sentence:**  
> If applied, this commit will ***your short commit message here***




### References
http://chris.beams.io/posts/git-commit/  
http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html  
https://wiki.typo3.org/CommitMessage_Format_(Git)
http://whatthecommit.com/

## Let's avoid uninformative commit messages!
![Messy Git Commits](http://imgs.xkcd.com/comics/git_commit.png)
