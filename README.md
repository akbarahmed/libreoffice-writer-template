# LibreOffice Writer Template

A design template for writing technical documentation with LibreOffice Writer.

The design looks the same on Mac OSX, Linux, and Windows as all fonts, colors, 
etc. are available on all platforms.

All of the styles included in this template are listed below. I did not 
customize every possible style as I updated the ones that I use when writing
technical documentation. Further, I am not a designer. I'm 100% confident that
a professional designer make a more attractive template, so please don't hate on
my design skills. :)

> This repo will not get many pushes as there's little reason to constantly 
> update a template.

Tested on:
- LibreOffice: 4.2
- Ubuntu Linux 14.04, Mac OSX 10.10 (Yosemite), Windows 7


## Installation

Installing the template involves downloading the `.ott` file then saving the
template to your `templates` directory. The final step is to copy the table
styles file to the LibreOffice `config` directory.

### Template file

Setting up the template file involves the same steps on Mac, Linux and Windows.

1. Download the [Tech Docs Template.ott](https://github.com/akbarahmed/libreoffice-writer-template/raw/master/Tech%20Docs%20Template.ott) file to 
   your `Downloads` folder. 
3. Navigate to your `Downloads` folder, then double-click  the 
   `Tech Docs Template.ott` file to open it in Writer.
4. Select `File`, select `Templates`, click `Save As Template...`.
5. In the **Template Manager** dialog box: 
    - Double-click `My Templates`.
    - Click `Save`.
    - Enter a template name of `Tech Docs Template` (or some other name that 
      you'd like to use for this template).
    - Click `OK`.

### Table AutoFormat file

> Close LibreOffice if it's open.

#### Install on Mac

1. Download the [autotbl.fmt](https://github.com/akbarahmed/libreoffice-writer-template/raw/master/autotbl.fmt) file to your `Downloads` folder.
2. Open a terminal an run the following commands:

```bash
# Backup your existing autotbl.fmt file
cp ~/Library/Application\ Support/LibreOffice/4/user/config/autotbl.fmt ~/Library/Application\ Support/LibreOffice/4/user/config/autotbl.fmt-bk

cp ~/Downloads/autotbl.fmt ~/Library/Application\ Support/LibreOffice/4/user/config/autotbl.fmt
```

#### Install on Linux

1. Download the [autotbl.fmt](https://github.com/akbarahmed/libreoffice-writer-template/raw/master/autotbl.fmt) file to your `Downloads` folder.
2. Open a terminal an run the following commands:

```bash
# Backup your existing autotbl.fmt file
cp ~/.config/libreoffice/4/user/config/autotbl.fmt ~/.config/libreoffice/4/user/config/autotbl.fmt-bk

cp ~/Downloads/autotbl.fmt ~/.config/libreoffice/4/user/config
```

#### Install on Windows 7

> Note: I'm unable to get the table AutoFormat file to work on Windows.

1. Download the [autotbl.fmt](https://github.com/akbarahmed/libreoffice-writer-template/raw/master/autotbl.fmt) file to your `Downloads` folder.
2. Open Windows Explorer and navigate to `C:/Users/<user name>/AppData/Roaming/LibreOffice/4/user/config`.
3. Make a copy of `autotbl.fmt`.
4. Copy the new `autotbl.fmt` file that you downloaded from the `Downloads` 
   folder to the LibreOffice `config` folder:

`C:/Users/<user name>/AppData/Roaming/LibreOffice/4/user/config`.


## Getting started

### Create new document

Let's start by creating a new document based on our template.

1. Open LibreOffice Writer.
2. Select `File`, select `New`, click `Templates`.
3. In the **Template Manager** dialog box:
    - Select the `Templates` tab. 
    - Double-click `My Templates`.
    - Double-click the `Tech Docs Template` file.


### Update the title property

1. Select `File`, click `Properties`.
2. Select the `Description` tab.
3. Change the `Title` field. The title is inserted into the footer of every 
   page.
4. Click `OK`.


## Template styles

### Paragraph styles

#### Default font style

- `Default Style`: The default font style that is used as the basis for other
  styles. Also used as the default style in the document. 
- `Text Body`: Similar to `Default Style`.

#### Headings

- `Title`: Document title at the top of 1st page.
- `Heading 1`: Level 1 heading. Typically used as a section heading.
- `Heading 2`: Level 2 heading. Typically used as a sub-section heading.
- `Heading 3`: Level 3 heading.
- `Heading 4`: Level 4 heading.
- `Heading 5`: Level 5 heading.

#### Blockquotes

- `Information`: Emphasize key points that the reader should learn. Blue.
- `Alert`: Highlight warnings and other danger areas. Red.
- `Hint`: Provide the reader with tips and tricks. Green.

### Code blocks

- `Code`: Highlight large code blocks.

#### Table fonts

- `Table Heading`: Provides a bold, centered font for table column or row 
  headings.
- `Table Contents`: Default font for values places within a table.

#### Image subtitle

- `Caption -> Image`: Small font size to write captions below an inserted image.

### Character styles

- `Inline Code`: Inline code is used to hightlight code placed in the middle of
  a normal sentence such as `y = x - 1`.

### Frame styles

- `Graphics -> Image`: Centers an image and prevents text wrapping.

### Table AutoFormat styles

- `Table`: Default table style for this template. 


## How to apply the various styles

> Mouse over the icons in the **Styles and Formatting** pane to view the text
> tip.

### Paragraph styles

1. Press `F11` to open the **Styles and Formatting** pane.
2. Click the `Paragraph Styles` icon in the **Styles and Formatting** pane.
3. Select the text you want to format, then double-click the style you want to
   apply.

### Character styles

1. Press `F11` to open the **Styles and Formatting** pane.
2. Click the `Character Styles` icon in the **Styles and Formatting** pane.
3. Select the text you want to format, then double-click the style you want to
   apply.

### Frame styles

1. Select `Insert`, select `Image`, click `From File...`.
2. Select an image, then click `OK`.
3. In the Writer document, select the newly inserted image.
4. In the **Styles and Formatting** pane, click the `Frame Styles` icon.
5. Double-click `Image`. (Hint: If `Image` is not visible, then expand 
   `Graphics`)

### Table AutoFormat styles

1. Press `Ctrl + F12` (or `Cmd + F12` on Mac) to open the **Insert Table**
   dialog box.
2. Press the `AutoFormat` button.
3. Select `Table`, click `OK`.
4. Change any other table settings you want to change, then click `Insert`.
