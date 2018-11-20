# How to contribute?
PRs are very much appreciated. You could e.g.:
* check the names of the files and rename them correctly (issue https://github.com/rugk/streetcomplete-quest-svgs/issues/1)
* upload new versions of the icons or new icons if they are changed in the original file and missing here.

See also other issues tagged with ["help wanted"](https://github.com/rugk/streetcomplete-quest-svgs/labels/help%20wanted).

## Split SVG file

In order to split the files, just follow [this guide](https://graphicdesign.stackexchange.com/questions/18088/exporting-an-object-as-svg-from-inkscape):
1. Click on icon.
2. Ctrl+Shift+R to resize page to drawing or selection.
3. (recommend) `!` to revert selection and `Del` to delete other items.
3. File > Save As Copy or Ctrl+Shift+S
4. Save as "Optimized SVG" (and as the usual "Inkscape SVG" later in the other directory, if you want).

## Minimize SVG image

When the SVGs are saved as "optimized SVGs" you can still minimize them even more. To do so just use [SVGO](https://github.com/svg/svgo), e.g. in the [webinterface](https://jakearchibald.github.io/svgomg/). Enable "Multipass" in order to decrease the file size even more.

**Note:** Please compare the resulting sizes of the files and choose the smallest one. Sometimes maybe also Inkscape's optimizer can be better than SVGO.
So pay attention: When the web GUI shows a red percentage that means the file size increased!

## Upload to the OpenStreetMap wiki

1. Use the usual upload options (e.g. when adding an image via the visual editor or [this special page](https://wiki.openstreetmap.org/wiki/Special:Upload).
2. Upload the **optimized versions** (from the [optimized dir](optimized/)) and **rename** them by replacing the `ic` with `StreetComplete`, so it is easier to find them. Apart from that, keep the original name.
3. Add the ["StreetComplete Quest Icon" category](https://wiki.openstreetmap.org/wiki/Category:StreetComplete_Quest_Icon), so all those images can be seen there.
4. Add a decription similar to this one with backlinks and all this legal:
   ```
   Quest icon of the app [[StreetComplete]] showing […image description goes here…].
   
   license: [https://creativecommons.org/licenses/by-sa/4.0/ CC-BY-SA 4.0] by [[User:Westnordost|Tobias Zwick]]<br>
   source: https://github.com/westnordost/StreetComplete/blob/master/res/quest_icons.svg
   [[Category:StreetComplete Quest Icon]]
   ```
   (This does already include step 3, i.e. the last line adds the category.)

