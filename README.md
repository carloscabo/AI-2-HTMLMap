AI-2-HTMLMap
============

AI-2-HTMLMap is an Adobe Illustrator Script that exports path items in your .AI document as standard HTML MAP Area coordinates. Perfect for building complex Image Maps directly in Illustrator or exporting complex shapes.

![AI-2-HTMLMap Screenshot](/readme-images/script-snapshot.png "AI-2-HTMLMap Screenshot")

Usage instructions
==================

  1. Be sure your Adobe Illustrator document units measurement is set to _**"Pixels"**_. You can check it at _**File > Document setup**_.

  2. For optimal results, set your document dimensions to the same width and height of the image you will use in the image map. If you are planning to export the image as PNG / GIF / JPEG directly from Illustrator please check the _**tips & tricks**_ section below.

  3. Before launching the script, select the paths you want to export as _**areas**_ in the resulting image map. No matter if you have layers or other items in the document, but be sure to select only _**paths**_ (nor bitmap images, neither symbols...). **This script works only with paths!.**

  4. Run the script dropping it in Adobe Illustrator, or selecting it in _**File > Scripts > Other script**_.

  5. Once you press the _**"Generate map"**_ button the script will show a dialog window with the HTML code for the image map.

  6. Copy + paste the HTML code in your project and remember to adjust what you need (like the path to the image, the alt attributes for the areas...).

Tips & Tricks
=============

![Named paths](/readme-images/path-names.png "Named paths")

  - By default the _**href**_ of the area will take the name of the path in Adobe Illustrator. You can set your own path names in the _**Layers palette**_ to help you to identify each _**area**_ in the resulting image map.

  - If you leave your path unnamed the _**areas**_ will be named sequentially... (#1, #2, #3...). Same occurs with _**alt**_ attributes.

  - By default all paths will be exported as _**shape="polygon"**_ if you want a path to be exported as _**rect**_ or _**circle**_ add the words to the path name separated from the rest of the name by one space. Take a look to the _**"AI_paths_to_HTML_MAP.ai"**_ file.

  - Remember that the _**circle**_ shapes must be perfectly circular. HTML Image Maps don't support ellipsoidal shapes.

  - If your path has hundreds of points you'll get a huge coordinate string. In some situations could be useful to reduce the complexity of the path. You can do it in Illustrator using the _**Object > Path > Simplify...**_ option.

  - If you plan to export your image to use it in your image map its a good practice to add a background layer with a rectangle with the same size of the document. Illustrator trims away empty pixels when exporting to PNG / JPEG using the _**File > Export**_ command.
