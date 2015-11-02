# ossec.github.io

This site is built with Sphinx using the code base in ossec.github.io/_project.
To visit the finished website, go to http://ossec.github.io.  Most of the website
shoudl remain the same over time except when have in OSSEC releases or want to add
a blog entry.  

## Updating the Downloads page

1. cd to _project/
1. Open the downloads.rst file
2. Make changes to links where necessary.
3. Run *make clean* then *make html*.
4. Open _project/_build/html/index.html in a browser to see the new website.
5. Repeat steps 2-4 as necessary until the Downloads page looks right.
6. Replace the ossec.github.io/downloads.html with _project/_build/html/downloads.html
7  Run *make clean*.
8. cd to the top level ossec.github.io
9. Push all the revisions to ossec.github.io.

## Adding a blog entry

1. cd _project/blog/posts
2. Create a file using the naming convention *YYYY-mm-dd-TITLE.rst* in the blog/posts directory.
2. Replace *TITLE* with the title of your blog.
3. Add a section at the top of the blog file that looks like this:
   <pre>
       .. post:: MMM DD, YYYY
           :tags: your tags
           :category: your categories
           :author: your name

       =====
       TITLE
       =====
   </pre>
4.  Replace MMM with the month abbreviation of your blog, e.g. Jan, Feb, etc.
5.  Replace DD with the day number, e.g. 01, 02, 03, 3tc.
6.  Replace YYYY with the year. Note for steps 4-6 check the files in blob/posts for examples.
7.  Fill in the *your tags*, *your categories* and *your name* sections.  
8.  Write the blog content below your TITLE section.
9   cd to _project/  
9.  Run *make clean* then *make html*.
10. Open _project/_build/html/index.html in a browser to see the new website.
11. Repeat steps 7-10 until you blog content looks right.
12. Replace ossec.github.io/blog.html with _project/_build/html/_blog.html.
13. Copy the HTML version of your blog from _project/_build/html/blog/posts to ossec.github.io/blog/posts/
14  Run *make clean*.
15. cd to the top level ossec.github.io
16. Push all the revisions to ossec.github.io.

