# rachelloves.nyc

## How to create a new blog post

1. Open VS Code
2. Create a new file in the `content` directory - ex: `2022-01-17-my-new-post.md`
3. Add blog metadata to top of text area:

```
+++
title = "My New Post"
+++
```

## Things to do in Terminal.app

- `cd ~/Projects/rachelloves.nyc` - to get to your blog dir
- `zola serve` - to start the development server
- `code .` - to open vscode for this projects
- see git cheatsheet

## Git cheatsheet

1. `git status` - look for "untracked" changes
2. `git add .` - to add all untracked changes to commit
3. `git commit -am "My change message"` - to commit changes
4. `git push origin head` - to publish your changes to your blog!
5. `git pull` - to bring in any changes from someone else - should commit any changes first
