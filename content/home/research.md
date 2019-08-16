+++
# A Projects section created with the Portfolio widget.
widget = "portfolio"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 30  # Order that this section will appear.

title = "Research"
subtitle = ""

[content]
  # Page type to display. E.g. project.
  page_type = "project"
  
  # Filter toolbar (optional).
  # Add or remove as many filters (`[[content.filter_button]]` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove toolbar, delete/comment all instances of `[[content.filter_button]]` below.
  
  # Default filter index (e.g. 0 corresponds to the first `[[filter_button]]` instance below).
  filter_default = 0
  
   # [[content.filter_button]]
   #  name = "All"
   #  tag = "*"
  
   # [[content.filter_button]]
   #  name = "Deep Learning"
   #  tag = "Deep Learning"
  
   # [[content.filter_button]]
   #  name = "Other"
   #  tag = "Demo"

[design]
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns = "2"

  # Toggle between the various page layout types.
  #   1 = List
  #   2 = Compact
  #   3 = Card
  #   5 = Showcase
  view = 5

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
&emsp;&emsp;Under the advisement of [Dr. Chris Callison-Burch](https://www.cis.upenn.edu/~ccb/) with the School of Engineering and Applied Science and [Dr. Emily Falk](https://www.asc.upenn.edu/people/faculty/emily-falk-phd) with the Annenberg School for Communication at the University of Pennsylvania, my PhD research project is a cross discipline collaboration between Natural Language Processing (NLP) and Cognitive Science called Motivational Boost.
<br>
<br>
<br>

{{< youtube AsPhEZr6bsk >}}

<br>
<br>
<br>
&emsp;&emsp;Whereas prior work has looked at features of naturally occurring language and how persuasive that language turns out to be, Motivational Boost is novel in looking for casual explanations behind what makes text persuasive by manipulating linguistic features in content messages and measuring the perception of persuasion, motivation, relevance, intention, and confidence on the ability to positively change behavior.  As an extension to work done by Lillian Lee in “[Winning Arguments: Interaction Dynamics and Persuasion Strategies in Good-faith Online Discussions](https://chenhaot.com/pubs/winning-arguments.pdf)," (Tan et al, 2016) we take the linguistic features observed in a subreddit called “Change my View” (CMV) to manipulate motivational messages on parenting.  CMV is an argumentation platform on Reddit where a stance on a topic is posted by an original poster (OP) and responders can make reasonable objections through the civil discourse this platform provides.  At the end of an argumentation thread, the original poster rates which responder’s viewpoint changed their mind, giving researchers a structured dataset that includes language used to persuade and ratings of success.
