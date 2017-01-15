# Fireside Magazine
This is the source for Fireside Magazine. It runs on (Jekyll)[https://jekyllrb.com], and is served off (Github Pages)[https://pages.github.com]. The idea is that, with a little bit of Markdown and Git knowledge, we can make Fireside production as simple as editing some plain text flies in a folder, and making a push to (the Fireside git repository)[https://github.com/firesidefiction].

# Writing and editing content in Fireside
You can update the content on fireside magazine by editing the text files inside the `_posts` folder.
Fireside is written and edited in raw text files, using Markdown, a plain text formatting syntax system. This allows editors to focus on consistent, semantic formatting of the content, rather than worry about presentation, which can change from platform to platform and over time.

Our site's robot helper, Jekyll, automatically converts raw text files written in Markdown into HTML when we publish. This guide outlines the rules we need to follow to ensure that Jekyll doesn't get confused. Robots are so needy. Anyway, onward.

Each Fireside document is composed of three parts:
- The Front Matter
- The Content
- The Author Bio

Let's go through each one individually.

## Front matter
Every piece of content that we post to Fireside *must* include front matter. The front matter *must* be the first thing in the document, and *must* be surrounded by three dashes. The front matter *must* be in YAML format, which is simply: `parameter: value`.

Here's what it looks like: 
> ---
> layout: story | post | article
> title:  The Title of The Thing
> author: Author Name
> date:   2017-mm-de 12:00:01 -0500
> category: short story | flash fiction | announcement | essay
> permalink: the-title-of-the-thing | /issue38/chapter/25/
> published: true | false
> teaser: "A short summary or teaser for the piece of content. Can be a direct quote form the piece, or something new. This will show up on the homepage."
> art: the-title-of-the-thing.jpg
> caption: A description of the artwork for screen readers
> artist: Galen Dara
> ---

Simple, right? The above template includes all the parameters available, and all the values possible, separated by pipes ( | ). You can copy/paste it directly into your document as a starting point. 

Some of the parameters are required, and some are optional. If you're not going to use an optional parameter, simply delete it — but don't just leave it blank. That will confuse the robot.

The parameters in the front matter are pretty self-explanatory,  but let's go over what each one means one by one anyway.

### `layout: story | post | article`
The `layout` parameter is **required**. It tells Jekyll what this document should look like.
Only one of three values are allowed: `story` for fiction, `post` for news items, and `article` for nonfiction.

### `title:  The Title of The Thing`
The `title` parameter is **required**. It tells Jekyll what the display title of the content should be.
This parameter allows free-form text. (The only exception is colons. Since YAML uses colons for its notation, if we need a colon in our text, we need to escape it as `&#58`, or consider using something else, like an em dash.)

### `author: Author Name`
The `author` parameter is **required**. It tells Jekyll who wrote the thing.
This parameter allows free-form text.

### `date: 2017-mm-dd 12:00:01 -0500`
The `date` parameter is **required**. It tells Jekyll what publishing date to display along with the content.
This parameter needs the date to be in the particular format shown:  `yyyy-mm-dd hh:mm:ss: -0500`. The date is important, but we don't really care about the time, so we always leave that set to `12:00:01 -0500`, which is midnight on Eastern Standard Time.

### `category: short story | flash fiction | announcement | essay`
The `category` parameter is **required**. It tells Jekyll what label to use when presenting the content on the site. 
This parameter can take free-form text, but Jekyll will give the four categories listed — `short story`, `flash fiction`, `announcement`, and `article` — special treatment, so we want to stick to those. If you want to add a new category, let Pablo know, so that he can tell Jekyll to treat it special, too.

### `permalink: the-title-of-the-thing | /issue38/chapter/25/`
The `permalink` parameter is **required**. It sets a custom permalink piece of content.
For new content, we will be using clean, human-readable URLs that match the title of the piece of content. For instance, if the `permalink` parameter is set to `dragon-soap`, the URL for the story will be `fireisdefiction.com/dragon-soap`. For content that we're migrating from Wordpress, we will want to keep the content's current URL, so that we don't break existing links, so we use everything after the 'fireisdefiction.com' part of the Wordpress URL.

### `published: true | false`
The `published` parameter is **required**. It tells Jekyll to either publish the piece of content, or ignore it if it's not ready yet.
Only two values are allowed: `true` or `false`.


### `teaser: "A short summary or teaser for the piece of content. Can be a direct quote form the piece, or something new. This will show up on the homepage."` 
The `teaser` parameter is **optional**. It should be a short summary or teaser for the piece of content. It can be a direct quote form the piece, or something new. This will show up on the homepage.
This parameter allows free-form text.

### `art: the-title-of-the-thing.jpg`
The `art` parameter is **optional**. It tells Jekyll the file name of an accompanying featured illustration.
This parameter takes a filename, which should be the same as the permalink based on the title of the piece, and it must include the file extension (.jpg, for instance).

### `caption: A description of the artwork for screen readers`
The `caption` parameter is **required** if you also include the `art` parameter. It sets a description of the image as alt-text for screen readers. It should be a short description of the content of the image, itself, as opposed to a description of what the image is. For instance, it should read "A woman crouching in a swamp, with a rifle in her hand." rather than "Illustration for the story Dragon Soap."
This parameter allows free-form text.

### `artist: Galen Dara`
The `artist` parameter is **required** if you also include the `art` parameter. It sets the artist name for the featured illustration.
This parameter allows free-form text.

## Content
The content section is where the, um, content of the piece goes. This is where we use markdown notation to format the text according to its meaning (rather than according to its visual style). We'll use the following conventions and notation for writing markdown for Fireside:
- use single underscores or asterisks for _emphasis_
- use double underscores or asterisks for **strong emphasis**
- write links like this: [link text](http://url.com)
- use four dashes for section breaks: ---- 
- use a > for blockquotes
- add a blank line between paragraphs, otherwise the line will be a regular carriage return, not the start of a new paragraph.

## Author Bio