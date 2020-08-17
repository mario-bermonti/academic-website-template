
# Table of Contents

-   [Academic Website Template](#org6537545)
-   [Building your website](#org6879612)
-   [Modifying the website](#orge288457)
    -   [Important note](#orgfbf6377)
    -   [Adding the website's basic information](#org066e6cc)
    -   [Adding content](#org2375670)
        -   [Long version](#org0f0dfc5)
        -   [Short version](#orgd26f83a)
    -   [Further customization](#org097bbc0)
    -   [Note about modifying your website](#orgf9bbe6d)
        -   [Modify the website online](#org012e72f)
        -   [Modify the website on your computer](#org670996b)
-   [Contributing to this project](#org68b7f2c)
-   [Other options](#org5b3fca5)
-   [Author](#orgedf564f)
-   [License](#orgadf2b54)


<a id="org6537545"></a>

# Academic Website Template

This template was designed to provide an easy way to create academic 
websites. The goal is to lower the barrier to create webpages
for scholars with limited knowledge about programming.

This is achieved by separating content from form. This way you can simply
add your content and everything else is done for you. This template is
heavily influenced by [Academic pages](https://github.com/academicpages/academicpages.github.io) and [Simon Ho's website](https://www.simonho.ca/).

This website template is created with [Jekyll](https://jekyllrb.com/) - a static site generator -
and uses the [minimal mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/). The template was created so that 
it's easy to deyloy to [Github Pages](https://pages.github.com/), but you can make simple
modifications to deploy it on other services (see the [Jekyll documentation](https://jekyllrb.com/docs/deployment/)).


<a id="org6879612"></a>

# Building your website

1.  Create your own copy of this website by [forking](https://guides.github.com/activities/forking/) this GitHub repo
2.  [Unwatch](https://docs.github.com/en/github/managing-subscriptions-and-notifications-on-github/managing-your-subscriptions#unwatch-a-repository) the repo
3.  [Rename the repo](https://docs.github.com/en/enterprise/2.14/user/articles/renaming-a-repository) to <username>.github.io ([see step 3 of this guide](https://docs.github.com/en/github/working-with-github-pages/creating-a-github-pages-site-with-jekyll#creating-a-repository-for-your-site))
4.  Your website should be live at
    [https://<username>.github.io/](https://) ([see step 7 of this guide](https://docs.github.com/en/github/working-with-github-pages/creating-a-github-pages-site-with-jekyll#creating-a-repository-for-your-site))


<a id="orge288457"></a>

# Modifying the website


<a id="orgfbf6377"></a>

## Important note

There are two ways to modify your website. Each has pros and 
cons and require using different tools. You should make you decision
based on how comfortable you feel with the tools required for 
each option, but most importantly, how likely you are of using
them for other things. It may not be useful to learn a new tool
if you're only going to use it once. 

The two options are using GitHub's webpage or using Git locally. I
will discuss them very briefly to help you make your decision.
You can read the information in the section below "Note about modifying
your website"


<a id="org066e6cc"></a>

## Adding the website's basic information

This information is configured in
the `_config.yml` file. Here you can add information like the website's name,
your name, links to your research platforms, and many other information. 
Explore the different options to find everything that can be modified.


<a id="org2375670"></a>

## Adding content

Most pages incorporate their content from two sources: the actual 
file (e.g., `Research.md`) and the `yaml` file with the same name that 
can be found in the `_data` directory. 

This helps facilitate the process of adding new information because
the `yaml` files are very easy and intuitive to use, even if you don't know
any programming. These files follow a *bullet* or outline format and just
require you to *list* the contents you want displayed in your page.

For example, the Research page presents all the information that you include
in the `Research.md` file and then it includes the research projects
you have listed in the `research.yml` file. This makes it easier to 
continually add new research projects in the `yaml` file and keep your 
webpage updated.


<a id="org0f0dfc5"></a>

### Long version

If you know your way aroung Jekyll or similar platforms, you can skip
to the next section *Short version*.

This is the longer version and has all the details about managing your
website and should get you through, even if you don't know anything about
programming.

-   Add content to existing pages

    -   Regular content
    
        You can find the current pages in the `_pages` directory. To add new content,
        just write it in the file and save it. Also modify the page's metadata
        at the top of the page if you need to.
        
        If you would like to change the name of the page in the menu bar, you 
        have to modify it in the `navigation.yml` file that is in the `_data` directory.
    
    -   Yaml content
    
        The Research, Publications, Talks, and Software pages list the relevant 
        information by collecting it from its associated `yaml` file. These
        files are located in the `_data` directory and have the same name
        as the page (e.g., Research).
        
        To modify its content, just substitute the current information
        with your information. Keep the "" if there are any. Optional 
        fields are identified with comments.
    
    -   Featured rows
    
        The home and research pages contain a feature row to highlight your
        interests. To modify these rows, you have to provide the required
        information in each page. You can check the [theme's webpage](https://mmistakes.github.io/minimal-mistakes/docs/helpers/#feature-row)
        for more details.

-   Add new pages

    -   Create a `markdown` file in the `_pages` directory and add the content.
    -   Add metadata at the top of the file
        Hint: create a copy of an existing page and add the new content
    -   Add the page to the menu bar, by adding it to the `navigation.yml` 
        file. Follow the format of other entries and add the name of the tab
        and add where the file will be saved to (permalink).

-   Remove existing pages

    -   Delete the page from the `_pages` directory
    -   Delete the entry from the `navigation.yml`

-   Adding files for download

    Add the files you need to be available in the website (e.g., CV, pdf
    for downloading) in the `downloads` directory.

-   Creating blog posts

    -   Blog's home page
    
        To modify the blog's home page, just add your content to the `blog.md`
        file in `_pages`.
        
        Hint: If you only want the blog, you will have to remove all other
              pages and set the blog's home as the website's homepage.
    
    -   Blog posts
    
        Blog posts are in the `_posts` directory. You can remove the ones
        that are there for illustration purposes. They are all from the 
        minimal mistakes theme project template.
        
        To add new blog posts, just create a new `markdown` file that meets the
        name and metadata requirements and add your content. See the [Jekyll's](https://jekyllrb.com/docs/posts/) 
        webpage for more details.


<a id="orgd26f83a"></a>

### Short version

-   Add content to existing pages

    The Research, Publications, Talks, and Software pages get their contents from
    their `markdown` and associated `yaml` file. So you have to modify
    both files.

-   Featured rows

    The Home and Research pages contain a feature row to highlight your
    interests. To modify these rows, you have to provide the required
    information in each page. You can check the [theme's webpage](https://mmistakes.github.io/minimal-mistakes/docs/helpers/#feature-row)
    for more details.

-   Add and remove pages

    Just create a `markdown` file in the `_pages` directory, add the
    metadata, and content. You also have to modify the `navigation.yml` 
    file.
    
    To remove pages, just delete the page from the `_pages` directory and
    delete the entry from the `navigation.yml`.

-   Adding files for download

    Add the files you need to be available in the website (e.g., CV, pdf
    for downloading) in the `downloads` directory.

-   Blog

    To modify the blog's home page, just add your content to the `blog.md`
    file in `_pages`.
    
    Blog posts are in the `_posts` directory. You can remove the ones
    that are there for illustration purposes. They are all from the 
    minimal mistakes theme project template.
    
    To add new blog posts, just create a new `markdown` file that meets the
    name and metadata requirements and add your content. See the [Jekyll's](https://jekyllrb.com/docs/posts/) 
    webpage for more details.


<a id="org097bbc0"></a>

## Further customization

The website has many more features. Please read
[Jekyll's](https://jekyllrb.com/docs/) and [minimal mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/) documentation for 
learning how to modify how the website looks and how it's structured.


<a id="orgf9bbe6d"></a>

## Note about modifying your website


<a id="org012e72f"></a>

### Modify the website online

You can use Github's webpage to modify your website. This is
the easiest method and may very well suit your needs. You won't have 
to install additional software and can modify your website from any
computer or device (e.g., tablet) without worrying much about anything
else. However, you won't be able to preview the changes to your website
before making them public. 

If you don't know what Git is or you don't feel comfortable with programming,
then this may be the best option for you.


<a id="org670996b"></a>

### Modify the website on your computer

This option requires installing a few software and learning to use 
them. You will also need to learn to use a 
text editor (e.g., [spacemacs](https://www.spacemacs.org/) [my favorite :) ], [vim](https://www.vim.org/), [atom](https://atom.io/), [notepad](https://notepad-plus-plus.org/))

This requires installing the following software:

-   [Ruby](https://www.ruby-lang.org/en/documentation/installation/)
-   [Jekyll](https://jekyllrb.com/docs/)
-   [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
-   Text editor (many computers have at least one installed by default)

After you have installed the required software, you need to [Clone](https://guides.github.com/activities/forking/#clone) this
repo to your computer. You should now be able to modify add content
to your website.

After making changes, preview them on your local computer following this
[guide](https://jekyllrb.com/docs/). To make your changes public, you have to push them to GitHub using
Git.


<a id="org68b7f2c"></a>

# Contributing to this project

All contributions are welcome!

You can help out by writing documentation or tutorials on how to modify
certain things, report bugs or errors in code or documentation, fixing bugs,
or by providing ideas. This is a beginner friendly project!

You are welcome to communicate any errors by [submitting an
issue](https://github.com/mario-bermonti/academic-website-template/issues) on Github.

To fix bugs, clone the repository, add your contribution, 
and submit a [pull request](https://github.com/mario-bermonti/academic-website-template/pulls).

If have suggestions on how to improve the website design (e.g., default
tabs, theme, etc.), please open an [issue on Github](https://github.com/mario-bermonti/academic-website-template/issues) or [email me](mailto:mbermonti1132@gmail.com). Please
keep in mind that the template should be general enough that works for
most people and only suggestions that will benefit most people will be
incorporated.


<a id="org5b3fca5"></a>

# Other options

-   [Matthew Kirby's Academic template](https://github.com/matthewkirby/academictemplate) (I actually discovered this one too late)
-   [Academic pages](https://academicpages.github.io) (it didn't work for me)


<a id="orgedf564f"></a>

# Author

This project was developed by Mario E. Bermonti-Perez as part of
his academic research and activities. Feel free to contact me at [mbermonti@psm.edu](mailto:mbermonti@psm.edu) or
[mbermonti1132@gmail.com](mailto:mbermonti1132@gmail.com)


<a id="orgadf2b54"></a>

# License

This project is based on the [minimal mistakes starter repository](https://github.com/mmistakes/minimal-mistakes/) 
and is licensed under the MIT license, just as the original project.

Please read the `LICENSE` file for more details.

