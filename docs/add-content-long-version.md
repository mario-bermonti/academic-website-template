
# Table of Contents

-   [Academic Website Template](#org985a391)
    -   [Adding content to your website](#org4bb9e11)
    -   [Further customization](#orgb10c7c4)
    -   [Other useful resources](#org103c2ef)


<a id="org985a391"></a>

# Academic Website Template


<a id="org4bb9e11"></a>

## Adding content to your website

This is a detailed version of how to add content to your site. It has all
the details about managing your website and should get you through,
even if you don't know anything about programming.

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
        and add where the file will be saved to (permalink). If no permalink is
        specified then it should just be the name of the file.

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
        
        Hint: If you only want the blog and are not interested in the complete 
              website, you will have to remove all other pages and set the
              blog's home as the website's homepage.
    
    -   Blog posts
    
        Blog posts are in the `_posts` directory. You can remove the ones
        that are there for illustration purposes. They are all from the 
        minimal mistakes theme project template.
        
        To add new blog posts, just create a new `markdown` file that meets the
        name and metadata requirements and add your content. See the [Jekyll's](https://jekyllrb.com/docs/posts/) 
        webpage for more details.


<a id="orgb10c7c4"></a>

## Further customization

The website has many more features. Please read [Jekyll's](https://jekyllrb.com/docs/) and
[minimal mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/) documentation for learning how to modify
how the website looks and how it's structured.


<a id="org103c2ef"></a>

## Other useful resources

-   [Create your Academic Website in Jekyll and Host it on Github](http://svmiller.com/blog/2015/08/create-your-website-in-jekyll/)
-   [Jekyll Academic Quickstart](https://ncsu-libraries.github.io/jekyll-academic-docs/)

