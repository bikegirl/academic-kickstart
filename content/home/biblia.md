+++
# A Projects section created with the Portfolio widget.
widget = "portfolio"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = false  # Activate this widget? true/false
weight = 90  # Order that this section will appear.

title = "Biblia"
subtitle = "pasajes favoritos"

[content]
  # Page type to display. E.g. project, widget_page.
  page_type = "biblia"
  
  # Filter toolbar (optional).
  # Add or remove as many filters (`[[content.filter_button]]` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove toolbar, delete/comment all instances of `[[content.filter_button]]` below.
  
  # Default filter index (e.g. 0 corresponds to the first `[[filter_button]]` instance below).
  filter_default = 3
  
  [[content.filter_button]]
    name = "All"
    tag = "*"
  
  [[content.filter_button]]
    name = "Isaiah"
    tag = "Isaiah"
  
  [[content.filter_button]]
    name = "Romans"
    tag = "Romans"

  [[content.filter_button]]
    name = "Proverbs"
    tag = "Proverbs"

  [[content.filter_button]]
    name = "Acts"
    tag = "Acts"

  [[content.filter_button]]
    name = "Genesis"
    tag = "Genesis"

  [[content.filter_button]]
    name = "Daniel"
    tag = "Daniel"

  [[content.filter_button]]
    name = "Chronicles"
    tag = "Chronicles"

  [[content.filter_button]]
    name = "Corinthians"
    tag = "Corinthians"

  [[content.filter_button]]
    name = "Jeremiah"
    tag = "Jeremiah"

  [[content.filter_button]]
    name = "Phillipians"
    tag = "Phillipians"

  [[content.filter_button]]
    name = "Matthew"
    tag = "Matthew"

  [[content.filter_button]]
    name = "Psalms"
    tag = "Psalms"

  [[content.filter_button]]
    name = "Joel"
    tag = "Joel"

[design]
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns = "2"

  # Toggle between the various page layout types.
  #   1 = List
  #   2 = Compact
  #   3 = Card
  #   5 = Showcase
  view = 2

  # For Showcase view, flip alternate rows?
  flip_alt_rows = false

[design.background]
  # Apply a background color, gradient, or image.
  #   Uncomment (by removing `#`) an option to apply it.
  #   Choose a light or dark text color by setting `text_color_light`.
  #   Any HTML color name or Hex value is valid.
  
  # Background color.
  # color = "navy"
  
  # Background gradient.
  # gradient_start = "DeepSkyBlue"
  # gradient_end = "SkyBlue"
  
  # Background image.
  # image = "background.jpg"  # Name of image in `static/img/`.
  # image_darken = 0.6  # Darken the image? Range 0-1 where 0 is transparent and 1 is opaque.

  # Text color (true=light or false=dark).
  # text_color_light = true  
  
[advanced]
 # Custom CSS. 
 css_style = ""
 
 # CSS class.
 css_class = ""
+++