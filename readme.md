# Your resume, online!

![Demo](https://github.com/gonzal15/gonzal15.github.io/blob/main/A2%20Gif.gif)

## Purpose

The purpose of this ReadMe is to help you host your resume online as a static website. By the end of this tutorial, you should be able to:
- use Markdown with your Markdown editor to create your resume
- use Jekyll to generate a static website
- use GitHub and GitHub Pages to maintain and host your resume online

These goals align with the principles taught in Andrew Etter's book, *Modern Technical Writing*. As you read through the instructions, you will see references to his book and his justifications for why we do the things we do in this tutorial.

## Prerequisites

**Before you start**, you should have the following:

- A GitHub Account
- A Markdown editor, this ReadMe was written using [ghostwriter](https://github.com/KDE/ghostwriter)
- Jekyll, a static site generator. You can [view instructions here](https://jekyllrb.com/docs/installation/) for more information on how to install Jekyll according to your operating system

If you're new to using Markdown, check out the **More Resources** section of this ReadMe to get a link to a tutorial on using Markdown.

## Instructions

#### 1) Create your resume in Markdown

The first step is to open your Markdown editor and start creating your resume. If you have a resume already handy in a .docx or .pdf format, you can copy the information from there into your Markdown editor and make adjustments as needed.

Markdown is a lightweight markup language used to create and format simple text documents. While web pages are displayed to you using HTML (another markup language) writing HTML code can be a bit difficult, especially when starting out. Markdown files can be converted to an appropriate format that can be displayed as a webpage. The purpose of a lightweight markup language like Markdown is to have a more human-readable piece of code that others can look at.

This feature is pointed out by Andrew Etter in his book, and using a lightweight markup language as a technical writer is one of his principles. He notes that having something written in Markdown also makes it easier for collaboration. For example, when writing a ReadMe file that is to eventually be modified by different people with diverse skillsets, a lightweight markup language makes it easier for those people to make a meaningful contribution.

#### 2) Create a new website with Jekyll

Now that we have a Markdown-formatted resume, we want to get the files ready for when we eventually host it online. We can get a folder created locally on your computer with all of the relevant files we need using Jekyll.

Start by opening your computer's terminal. Then, enter the following command:  
```
jekyll new [name]
```
Where "name" is the name of the folder you want to create. Depending on the directory that you opened your terminal in, there should now be a folder there with the name you gave in the command. This folder contains all of the necessary files to host your website.

You may have noticed that the size of this folder is pretty small, and Andrew Etter notes this as a strength. Compared to dynamic websites, static websites don't require a lot of resources to create nor to host online. This makes them a quick and efficient option for showing text, which is desirable when the point of your website is only to show text!

#### 3) Create a repository for your website in GitHub

In order to host your website through GitHub Pages, you will need to create a repository in your GitHub account for it. Creating a repository is as simple as clicking the button in the top right corner of this page in GitHub where your profile picture is, going to "Your repositories", and then clicking the green button that says "New". The name of your repository should be in the following format:
```
yourGitHubUsername.github.io
```

GitHub provides a distributed version control system (DVCS), which helps keep track of what changes were made and by who. This accommodates the collaboration aspect mentioned earlier that Andrew Etter gave, but he also notes that a DVCS is preferred by software developers. As well, using a DVCS to store things such as a project's ReadMe ensures that the file can stay updated along with the code. By keeping things up-to-date, mistakes and errors can be avoided from both the writer side and the developer side.

#### 4) Update your folder with your resume

Specifically, we're going to update the file titled:
```
index.md
```

In this file, below the content at the top (called the "front matter") separated with its own dashes, you can copy and paste the contents of your Markdown-formatted resume into this space. Save and close the file.

#### 5) Upload your files to your repository

At the moment, the repository you created in step 3 is currently empty. Go to your repository's page. There should be a blue-shaded box for quick setup. From there, click on the option that says "upload an existing file". You will then be taken to a page where you can upload your files. From here, you can go ahead and upload all of the files from the folder you created in step 2. Be sure to commit your changes with the green button near the bottom!

#### 6) Celebrate

At this point, once you've given a few minutes after uploading your files, you should be able to view your resume at
```
yourGitHubUsername.github.io
```

Congratulations! You are now ready to share this link with prospective employers!

## More Resources

- A great Markdown tutorial can be [found here](https://www.markdowntutorial.com/).
- An overview of the basic syntax of Markdown can be [found here](https://www.markdownguide.org/basic-syntax/)
- *Modern Technical Writing*, by Andrew Etter, can be purchased from [Amazon](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)

## Authors and Acknowledgements

## FAQs

> Why host text online as a static website rather than saving and sending the text as files?

Files such as .docx or .pdf are saved and distributed once they are ready. A problem occurs when those files need to be updated. If someone has an older version of something you wrote and you need to get them the new and improved version, this can require creating a new file, notifying the person, etc. Unlike text files, hosting the text online provides the "one place of truth", and updates can be made in real time.

> I've hosted my resume, but my name at the top is showing up twice. How do I fix this?

Go to your repository, and edit the file named:
```
index.md
```
Recall from step 4 of the instructions that there is the section of the file that was referred to as the "front matter", identified with three dashes above and below. If you created a heading at the top of your resume with your name, delete this. In the front matter, add a new line that says within the dashes:
```
title: [your name]
```
Save this change. After a few minutes, your website should update and have your name only show up once.
