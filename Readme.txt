README~!
3-14-2016 - Some additional changes to routing in the requestHandler file were made to add argument ordering.
3-13-2016 - The dynamicPages controller and editpage view were just updated to allow multiple positions in the template views.

Head to getpit.com (subject to change, incomplete) for the full documentation.

PHP-MVCMS is a custom mvc framework augmented for the cms which is built using the mvc system. 

PHP-MVCMS is licensed under the GNU open source liscense.

This CMS is designed for developers who are familiar with mvc, it is not recommended for individuals with no web development experience! 

The project currently contains the MVC CMS and a simple demonstration blog application written in MVC to show how to interface with the system search and caching.

There are still notices and warnings which you may want resolve to make trouble shooting a more pleasant experience.


Limitations

Only pdo databases are supported at this point, there is no abstraction layer.

The site search only supports the English language due to the need for a different stemming solution per language.

Passwords are stored in plain text by default, this should be remedied by a security expert near you.

Todos:
The automatic responsive videos will need to have a check to ensure that they are videos.
Find a better solution for the javascript minifier.
Add password encryption.

Highlights

The admin system is mobile compatible. 

Ckeditor is used for page content and blog articles.

User system has 3 levels; public, author and admin which can be used anywhere being that is an auto loaded class.

Easy deployment requires an empty db and for the files to be unzipped to your public htdocs folder, the tables are setup automatically during the installation process.

Multiple menus can be setup and placed throughout your site independently. The template model can be loaded and used from within a mvc custom app which allows the menus to be uniform and updated throughout where ever they are placed.

 

Developer Notes

The micro mvc can be used independently of the cms and pages, and or content tables can be used by an mvc app so the system can index its content in the site search.

To develop an mvc application to be indexed in the site search you have 2 options.
1. (easiest & recommended) Use an article only. Columns required are: articlename, link, published, type and content columns. (description is also used if supplied)
2. (advanced) Use the page table and supply an articleid and article with content, a type and link (headline will be the title in the site search, content- searchable exact matches currently highlighed in results). In this case the sitemap and search can be used (.0 priority can be used to remove item from the sitemap).  



© 2016 Carl Turechek
Many libraries are used and documented in PHP-MVCMS, those copyrights and licenses should be honored as well.
