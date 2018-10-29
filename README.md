## Welcome to the AHA Board Website

This repository contains within it all the secret magicks of the All Hands Active Board.

- A list of all future and ongoing board- and member-suggested projects
- A list of accomplished projects
- An archive of board meeting minutes

Each board member has access to add their projects, or projects suggested to them by members. This README acts as the board website's grimoire - it can teach you everything you need to know about updating the board website.

## Contents

1. [Updating the Site](#updating-the-site)
  1. [Using the Command Line](#using-the-command-line)
  2. [Using Github Pages](#using-github-pages)
  3. [Markdown Cheatsheet](#markdown-cheatsheet)
2. [Posting Minutes](#posting-minutes)
3. [Resources](#resources)

## Updating the Site

There are two methods for updating the website. The preferred method is to [clone this repository](https://help.github.com/articles/cloning-a-repository/) so that you can [make and test your changes on your computer](#using-the-command-line) prior to pushing them to the live website.

The less preferred option is to [edit files in this repository](#using-github-pages) using your browser. Be careful if you choose this option, because your changes will go live on the website once you commit without giving you a chance to test them!

### Using the Command Line

#### System Requirements

1. [Install Git](https://help.github.com/articles/set-up-git/)
2. [Install Jekyll](https://jekyllrb.com/docs/installation/)

Jekyll requires Ruby, RubyGems, GCC, and Make. [See the Jekyll documentation for instructions on checking if you have these installed](https://jekyllrb.com/docs/installation/)

#### Setting up the Site

1. [Clone this repository](https://help.github.com/articles/cloning-a-repository/)
2. Change directory into your local repository (```cd mydirectory```)

You should now be able to run a test environment by typing ```jekyll serve``` in the command line and navigating to localhost:4000 in your browser.

#### Making & Testing Changes

Make changes to files using [Markdown](#markdown-cheatsheet) and your favorite text editor. After saving your changes, you can run ```jekyll serve``` on the command line and navigate to localhost:4000 to see your changes. ```jekyll serve``` allows you to see what your changes will look like on the live website once you commit and push your changes. Changes made on your computer will not go live on the website until you commit and push your changes.

#### Git Command Line Cheatsheet

- Check the status of your local repository (see what needs to be committed): ```git status```
- Add files to be committed: ```git add [filename]```
- Committing work: ```git commit``` - this will open up your terminal's text editor so you can write a commit message
  - For short commit messages, you can use ```git commit -m 'your commit message'```
  - Remember that commit messages should generally be short, but thorough, so that other people can figure out what you've done
- Pushing changes to the remote repository (and the website!): ```git push origin master```
- Pulling changes other people have made to your local repository: ```git pull origin master```

Github has comprehensive documentation on their help pages, which are found here: https://help.github.com/.

### Using Github Pages

If your local system (your computer) is not set up to use jekyll and git, you can use the [editor on GitHub](https://github.com/allhandsactive/board/edit/master/README.md) to maintain and preview the content for your website in Markdown files. _Previewing in Github does not allow you to see changes on the site before they go live!_ The "preview" function only allows you to review the markdown structure of your page before you commit.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown Cheatsheet

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
  - Unordered indented point
  1. Ordered indented point
- List

1. Numbered
  1. Ordered indented point
  - Unordered indented point
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

## Posting Minutes

The ```_drafts``` directory holds unpublished drafts of the meeting minutes, and contains a file called ```minutes-template.md``` that can be used to easly structure the meeting minutes that will be published to the website.

To create a draft, create a newfile in ```_drafts``` titled something like ```draft-filename.md```. Copy and past all of the text in the ```minutes-template.md``` file into your new file, and add your notes from the meeting. You can preview your draft on your computer by running ```jekyll serve``` or ```jekyll build --drafts``` and navigating to localhost:4000/draft-filename.md.

When you're ready to publish your draft, rename the file to ```YYYY-MM-DD-meeting-minutes.md```, and move the file to ```_posts```. You will need to [commit and push](#git-command-line-cheatsheet) the post to the remote repository to publish the minutes on the live website.

[Jekyll Posts Documentation](https://jekyllrb.com/docs/posts/)

## Resources

### Jekyll Documentation

If you're having problems with Jekyll, or need to know how to make a change that isn't described in this README, you can check the [Jekyll Docs](https://jekyllrb.com/docs/) - these are pretty comprehensive and should have the answer.

### Jekyll Themes

The AHA Board website uses the minima layout, which was selected in our [repository settings](https://github.com/allhandsactive/board/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Github & Git Support

Github has comprehensive documentation on their [help pages](https://help.github.com/).

You might also find the [Git Documentation](https://git-scm.com/doc) helpful.

### Github Pages Support or Contact

Having trouble with Github Pages? Check out the [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and they’ll help you sort it out.
