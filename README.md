AI-2-HTMLMap
============

AI-2-HTMLMap is an Adobe Illustrator Script that exports path items in your .AI document as standard HTML MAP Area coordinates. Perfect for building complex Image Maps directly in Illustrator or exporting complex shapes.

![AI-2-HTMLMap Screenshot](/readme-images/script-snapshot.png "AI-2-HTMLMap Screenshot")

Usage instructions
==================

  1. Be sure your Adobe Illustrator document units measurement is set to _"Pixels"_. You can check it at _File > Document setup_.

  2. For optimal results, set your document dimmensions to the same width and height of the image you will use in the image map. If you are planning to export the image as PNG / GIF / JPEG directly from Illustrator please check the _tips & tricks_ setion below.

  3. Before launching the script, select the path you want to export as _areas_ in the resulting image map. No matter if you have layers or other items in the document, but be sure to select only _paths_ (nor bitmap images, neither symbols...). This script works only with paths!.

  4. Run the script dropping it in Adobe Illustrator, or selecting it in _File > Scripts > Other script_.

  5. Once you press the _"Generate map"_ button the script will show a dialog window with the HTML code for the image map.

  6. Copy + paste the HTML code in your project and remember to adjust what you need (like the path to the image for instance).

Tips & Tricks
=============

  - By default the _href_ of the area will take the name of the path in Adobe Illustrator. You can set your own path names to help to identify each _area_ in the image map renaming the path in the _Layers palette_.

  - If you leave your path unnamed the _areas_ will be named sequentially... (#1, #2, #3...). Same occurs with _alt_ attribute.
  
  - By default all paths will be exported as _shape="polygon"_ if you want a path to be exported as _rect_ or _circle_ add the words to the path name.

  - Remember that the _circle_ shapes must be perfectly circular. HTML Image Maps don't support ellipsoidal shapes.
  
  - If your path has hundreds of points you'll get a huge coordinate string. In some situations could be usefull to reduce the complexity of the path. You can do it in Illustrator usign the _Object > Path > Simplity..._ option.
  
  - If you plan to export your image to use it in your image map its a good practice to add a background layer with a rectangle the same size of the document. Illustrator trims away empty pixels when exporting to PNG / JPEG using the _File > Export_ command.
