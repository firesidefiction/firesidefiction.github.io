# Fireside Magazine
This is the source for Fireside Magazine. It runs on [Jekyll](https://jekyllrb.com), and is served off [Github Pages](https://pages.github.com). The idea is that, with a little bit of Markdown and Git knowledge, we can make Fireside production as simple as editing some plain text flies in a folder, and making a push to [the Fireside git repository](https://github.com/firesidefiction).

# Getting set up
Before you can update the content on Fireside, you need to clone the git repository for the site to your computer or tablet. In order to do that you’ll need to set up a user account at [GitHub](https://github.com), and download the [GitHub Desktop app for Mac or Windows](https://desktop.github.com). If you’re working in iOS, you can download [Working Copy](https://workingcopyapp.com) instead.

## Setting up your local repository
First, install the appropriate git app on your system. Once that's done, and you've signed into the app using your GitHub credentials, it's time to 'clone' the repository.

### On macOS or Windows
Go to the [Fireside Magazine repo](https://github.com/firesidefiction/magazine), click the 'Clone or Download' button, then click 'Open in Desktop.' Your GitHub Desktop app should automatically launch, and present you with a save window. Once you've saved the repo somewhere on your system, you're ready to work.

### On iOS
In Working Copy, tap on the `+` sign and select 'Clone repository.' And select the 'firesidefiction: magazine' repository.

# Writing and editing content in Fireside
You can update the content on Fireside magazine by editing the markdown (.md) text files inside repository with any text editor.

The markdown files at the top level of the repository (the `magazine` folder) are used to create the main pages of the site, such as the about page, or the legal boilerplate.

The files inside the `_posts` folder are the files for Fireside's content: stories, articles, news items, as well as information about Fireside books.

(There are additional folders in the repository, but those are for generating the site, so there's no need to worry about them in order to write and edit content for the site.)

## Working with Markdown files on Fireside
Fireside is written and edited in raw text files using Markdown, a plain text notation system. This allows editors to focus on consistent, semantic formatting of the content, rather than worry about presentation, which can change from platform to platform and over time.

Our site's robot helper, Jekyll, automatically converts raw text files written in Markdown into HTML when we publish. There are a few rules we need to follow to ensure that Jekyll doesn't get confused. Robots are so needy. Anyway, onward.

All Fireside documents *must* be named using the following naming convention:

`yyyy-mm-dd-title-of-the-thing.md`

The year, month, and date must correspond to the day it was (or will be) published, and the rest of the text should be the title of the piece. The `.md` file extension indicates it's a Markdown file.

Each Fireside document is composed of three parts:
- The Front Matter
- The Content
- The Author Bio

Let's go through each one individually.

## Front matter
Every piece of content that we post to Fireside *must* include front matter. The front matter *must* be the first thing in the document, and *must* be surrounded by three dashes. The front matter *must* be in YAML format, which is simply: `parameter: value`.

Here's what it looks like:
like:

> ---
>
> layout: story | post | article | book
>
> title:  "The Title of The Thing"
>
> author: Author Name
>
> date:   2017-mm-de 12:00:01 -0500
>
> category: short story | flash fiction | announcement | essay | book | serial
>
> permalink: the-title-of-the-thing | /issue38/chapter/25/
>
> published: true | false
>
> teaser: "A short summary or teaser for the piece of content. Can be a direct quote form the piece, or something new. This will show up on the homepage."
>
> art: the-title-of-the-thing.jpg
>
> caption: "A description of the artwork for screen readers"
>
> artist: Galen Dara
>
> ---

Simple, right? The above template includes all the parameters available, and all the values possible, separated by pipes ( | ). You can copy/paste it directly into your document as a starting point.

Some of the parameters are required, and some are optional. If you're not going to use an optional parameter, simply delete it — but don't just leave it blank. That will confuse the robot.

The parameters in the front matter are pretty self-explanatory,  but let's go over what each one means one by one anyway.

##### `layout: story | post | article | book`
The `layout` parameter is **required**. It tells Jekyll what this document should look like.
Only one of three values are allowed: `story` for fiction, `post` for news items, `article` for nonfiction, and `book` for book promo pages.

##### `title:  "The Title of The Thing"`
The `title` parameter is **required**. It tells Jekyll what the display title of the content should be.
This parameter allows free-form text. In order for all characters to read properly, the text of the title *must* be surrounded by double quotes.

##### `author: Author Name`
The `author` parameter is **required**. It tells Jekyll who wrote the thing.
This parameter allows free-form text.

##### `date: 2017-mm-dd 12:00:01 -0500`
The `date` parameter is **required**. It tells Jekyll what publishing date to display along with the content.
This parameter needs the date to be in the particular format shown:  `yyyy-mm-dd hh:mm:ss: -0500`. For new content, the date is important, but we don't really care about the time, so we always leave that set to `12:00:01 -0500`, which is midnight on Eastern Standard Time.

##### `category: short story | flash fiction | announcement | essay | book`
The `category` parameter is **required**. It tells Jekyll what label to use when presenting the content on the site.
This parameter can take free-form text, but Jekyll will give the five categories listed — `short story`, `flash fiction`, `announcement`, `essay`, and `book` — special treatment, so we want to stick to those. If you want to add a new category, let Pablo know, so that he can tell Jekyll to treat it special, too.

##### `permalink: the-title-of-the-thing | /issue38/chapter/25/`
The `permalink` parameter is **required**. It sets a custom permalink piece of content.
W will be using clean, human-readable URLs that match the title of the piece of content. For instance, if the `permalink` parameter is set to `dragon-soap`, the URL for the story will be `fireisdefiction.com/dragon-soap`. The title should be in lower case and spaces should be replaced by dashes.

##### `published: true | false`
The `published` parameter is **required**. It tells Jekyll to either publish the piece of content, or ignore it if it's not ready yet.
Only two values are allowed: `true` or `false`.

##### `teaser: "A short summary or teaser for the piece of content. Can be a direct quote form the piece, or something new. This will show up on the homepage."`
The `teaser` parameter is **optional**. It should be a short summary or teaser for the piece of content. It can be a direct quote form the piece, or something new. This will show up on the homepage.
This parameter allows free-form text. In order for all characters to read properly, the text of the title *must* be surrounded by double quotes.

##### `art: the-title-of-the-thing.jpg`
The `art` parameter is **optional**. It tells Jekyll the file name of an accompanying featured illustration.
This parameter takes a filename, which should be the same as the permalink based on the title of the piece, and it must include the file extension (.jpg, for instance).

##### `caption: A description of the artwork for screen readers`
The `caption` parameter is **required** if you also include the `art` parameter. It sets a description of the image as alt-text for screen readers. It should be a short description of the content of the image, itself, as opposed to a description of what the image is. For instance, it should read "A woman crouching in a swamp, with a rifle in her hand." rather than "Illustration for the story Dragon Soap."
This parameter allows free-form text. In order for all characters to read properly, the text of the title *must* be surrounded by double quotes.

##### `artist: Galen Dara`
The `artist` parameter is **required** if you also include the `art` parameter. It sets the artist name for the featured illustration.
This parameter allows free-form text.

## Content
The content section is where the, um, content of the piece goes. This is where we use markdown notation to format the text according to its meaning (rather than according to its visual style). We'll use the following conventions and notation for writing markdown for Fireside:
- use single underscores or asterisks for _emphasis_
- use double underscores or asterisks for **strong emphasis**
- write links like this: `[link text](http://url.com)`
- use four dashes for section breaks: ----
- use a `>` for blockquotes
- add a blank line between paragraphs, otherwise the line will be a regular carriage return, not the start of a new paragraph.

## Author Bio
The Author Bio Is currently hard coded into each story post. In addition, the author should be added to the `author.md` page.

## Artwork requirements and layout guidelines

All illustrations go in the `illustration` folder. They *must* measure 3200 x 1800 pixels and *must* be named `title-of-the-story.jpg` — all lower case, dashes instead of spaces.

All other images go in the `images` folder.

When a story is first published on the site, it takes the top position on the homepage. If the story has a featured image, the image will bleed off the screen, slide under the logotype of the magazine, and will butt up directly against the bottom of the site header. This is the same presentation we use on individual story pages.

Depending on what the top middle of the illustration contains, the logotype on the homepage could become obscured by the illustration, but that's OK—the bold presentation of the white icon over the red header is enough of an indicator for the magazine brand.

When the story with the illustration is no longer the newest item on the site, it will slide down the homepage. At that point the illustration shrinks to fit inside the red fiction box within the layout. This is just a scaling change—we're still not cropping the illustration.

For magazine layout purposes, we can lay a simple 3 x 4 grid over the illustration to block off some areas.

The top middle cell in the grid is where the magazine logotype will generally be placed. Avoid using that area for elements in the illustration which shouldn't be obscured.

The 1/3 width column created by the grid serves as a minimum width of the image. When we crop the image vertically, for ebook covers and for portrait-oriented phone wallpapers, we'll only be able to use  approximately one column's width.

We can crop wherever we want, obviously—we don't need to' just take the center column, or the left column, etc.—but the width of one column is the narrowest the crop will ever get.

# Publishing to the site
The Fireside website updates its contents as soon as you publish, or 'push', your changes to the 'magazine' repository on GitHub.com.

As you've been working on your device, your git client application has been keeping track of your changes. Each time you complete a significant chunk of work, you should write a short commit message describing the changes that you've made, and commit your changes to your local repository.

Once you've made all your changes and made all your commits, it's time to publish to the site. You do that by 'pushing' your local commits up to GitHub, where Jekyll will take care of taking your files and 'deploying' them to the site.
