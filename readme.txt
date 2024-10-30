=== Theme Companion ===
Contributors: Frumph
Tags: comicpress, css, editor, plugin, multisite, theme, companion, webcomic
Requires at least: 3.0
Tested up to: 3.4
Stable tag: 0.3.4
Donate link: http://frumph.net/

This plugin is used to assist in designing sites without editing the original style.css

== Description ==

Companion is intended to assist users designing their sites without editing their original style.css files.

Companion's features include:

* Editing CSS stylesheets that override the original style.css in the theme.
* Add custom information into the head area of your site/page for non-wpmu sites. - Does NOT activate for Multisite
  
= Please do *not* copy the entire style.css into the editor, the editor is used for placing specific element changes. If you want to change the background of your entire site you do =

body { background: #333333; }

#333333 being swapped for the color that you want to use.  
Notice that you do *not* need to replace the entire CSS element but just the portion you want to override / change.

== Changelog == 
= 0.3.4 =
Cleaned up notices/warnings, verified to work with WordPress 3.4

= 0.3.0 =
Verified to work with WordPress 3.1

= 0.2.9 =
Fixed the show style.css original etc.

= 0.2.7 =
Adjusted to use wp_upload_dir() to find the proper directories, i.e. wp 3.0 

= 0.2.6 =
Adjusted to work with 3.0/Multisite

= 0.2.5 =
Verified to work with WordPress 2.9.1

= 0.2.4 =
The color picker wasnt working out so removed it, fixed the plugindir variable.

= 0.2.3 =
Browser Selections types are now handled by body classes, so don't need them as css overrides, re-added the color picker to the help page.

= 0.2.2 = 
Rewrote the internals, removed the class because it wasn't working right with included files, /shrug, fixed to work with subdirectory installations

= 0.2.1 =
Added 'header.html' an edit option that allows you to put metatags custom php and javascript additions to the head area of your site.
fixed some naming conventions to be more appropriate to what your reading in the code
adjusted the help page to include some of the new 2.8.1 comicpress/commpress div id's and classes

= 0.2.0 = 
Fixed pathing for local xampplite installations and seperated WPMU better for pathing.
Prop Joe Kandra from [One Small Step](http://www.osscomic.com/)

= 0.1.9 = 
Fixed to be used with IE

= 0.1.8 =
New editor, using Edit Area now.  Tabbed the pages. 

= 0.1.7 = 
Changes the save location of your custom CSS files so they do not get overwritten when upgrading the plugin.

= 0.1.6 =
Fixes the WPMU path structure for blog.ids and wpmu installs using subdirectories.

= 0.1.4-5 =
Better pathing, fixes for installs in subdirectories. Removed the funkey acting color picker.
  
= 0.1.3 =
* Wordpress Site created the directory comicpress-companion and not comicpress_companion, adjusted.
* Also didn't like the core file in a subdirectory

= 0.1.1 =
* First release, works with Wordpress and WPMU ComicPress theme installations.

== Installation ==

1. Upload the `comicpress-companion` directory to the `/wp-content/plugins/` directory
1. Activate the plugin through the 'Plugins' menu in WordPress
1. Go to Appearance -> ComicPress Companion to start using the Companion.
1. Add CSS code that overrides your current style.css, add only the changed elements.

== Frequently Asked Questions ==

= The edit screen keeps saying that the file does not exist or the directory is not writeable even after I click save. =

Check the permissions on the plugin directory comicpress-companion/custom - For more information on this, contact your Webhost.  If you are
running WPMU make sure that the blogs.dir for the current blog's /files directory has the proper permissions as well (again as your webhost).

= I'm having another problem. =

If it's a serious problem, such as WordPress becoming non-functional or blank screens/errors after you perform certain operations, you will be asked to provide error logs for your server.  If you don't know how to get access to these, talk with your Webhost.  At that time just remove the plugin from the plugins/ directory.  If it still
continue's it is probably not a ComicPress Companion problem.

== License ==

Companion is released under the GNU GPL version 3.0 or later.

== Credits ==

Mondo thanks to John Bintz and Tyler Martin for their assistance, bug finding, and with coming up with ComicPress and ComicPress Manager in the first place.  

