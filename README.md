# Foldergallery module for CMS SilverStripe (2.4.x)
A lightweight folder based gallery module for the [SilverStripe CMS](http://silverstripe.org).

## Features
- easy upload of images via Ftp or the SilverStripe backend (Files & Images)
- thumbnails of uploaded images are created on the fly
- larger image scale appears on mouse click using a jQuery Colorbox effect
- image description is fetched from the image file name
- support for multiple albums included
- appearance of the thumbnails can be customized via template and CSS files
- multilingual support included (currently: English and German)

## Download
The last stable release of the `cwsoft-foldergallery v1.2.0` module for SilverStripe 2.4.x is available as [ZIP](https://github.com/cwsoft/silverstripe-cwsoft-foldergallery/archive/v1.2.0.zip) archive. This is the last release for the SilverStripe 2.4.x platform. Later releases of the cwsoft-foldergallery module do need SilverStripe 3.x and can be found at [GitHub](https://github.com/cwsoft/silverstripe-cwsoft-foldergallery#readme).

## License
The `cwsoft-foldergallery` module is licensed under the [GNU General Public License (GPL) v3.0](http://www.gnu.org/licenses/gpl-3.0.html).

## Requirements
The minimum requirements to get the cwsoft-foldergallery module running on your SilverStripe installation are as follows:

- SilverStripe ***2.4.5*** or higher (recommended last stable 2.4.x version)
- PHP ***5.2.2*** or higher (recommended last stable PHP 5.3.x version)

## Installation
1. download latest version for SilverStripe 2.4.x from [GitHub](https://github.com/cwsoft/silverstripe-cwsoft-foldergallery/zipball/v1.2.0)
2. unpack the archive on your local computer
3. upload the entire ***cwsoft-foldergallery*** folder to your SilverStripe root folder using your preferred Ftp program
4. update your SilverStripe database via `http://yourdomain.com/dev/build?flush=all`

## Usage
The required steps to create a single album page with the ***cwsoft-foldergallery*** module are explained below.

1. log into your SilverStripe backend and create a new page of type ***Folder Gallery*** (this creates a subfolder *assets/cwsoft-foldergallery* if not already exists)
2. now create a album subfolder inside *assets/cwsoft-foldergallery* (via Ftp or SilverStripe "Files & Images")
3. upload images to the created album folder (via Ftp or SilverStripe "Files & Images" section)
4. rename your images to `XX-your-image-description.ext` (XX image order 00..99)
5. this will create nice looking image descriptions in the form: "Your image description"
6. switch to the gallery page created in step 1
7. choose a subfolder for your album from the dropdown list
8. add a album header and some description via the WYSIWYG field
9. save and publish the gallery page

### Using albums
The ***cwsoft-foldergallery*** supports multiple albums. An album is basically a child page of a page of type `Folder Gallery`. The parent page will automatically create a list with the links to the individual albums available (child pages). 

To use the multiple albums features, create a page tree structure as follows:

	SilverStripe page tree:
	- Gallery (type: Folder Gallery)
	  + Album 2011 (type: Folder Gallery)
	  + Album 2012 (type: Folder Gallery)

A screenshot of the frontend is shown below.

![](.screenshots/cwsoft-foldergallery-frontend.png)

## Questions
If you have questions or issues with cwsoft-foldergallery, please visit the [SilverStripe](http://www.silverstripe.org/all-other-modules/show/20738) forum thread and ask for feedback.

***Always provide the following information with your support request:***

 - detailed error description (what happens, what have you already tried ...)
 - the cwsoft-foldergallery version used
 - your PHP and SilverStripe version used
 - information about your operating system (e.g. Windows, Mac, Linux) incl. version
 - information of your browser and browser version used
