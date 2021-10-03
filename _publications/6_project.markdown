---
layout: page
title: OptiDwell&#58; Intelligent Adjustment of Dwell Click Time
description: Nayyar A., <b>Dwivedi, U.</b>, Ahuja, K., Rajput, N., Nagar, S. and Dey, K. OptiDwell&#58; Intelligent Adjustment of Dwell Click Time. <i>International Conference on Intelligent User Interfaces (IUI) 2017.</i>
img: /assets/img/optidwell.png
importance: 3
type: Full Paper
pdf: /pdfs/optidwell-intelligent-adjustment(3).pdf
abstract: Gaze based navigation with digital screens offer a hands-free and touchless interaction, which is often useful in providing a hygienic interaction experience in a public kiosk scenario. The goodness of such a navigation system depends not only on the accuracy of detecting the eye gaze but also on the ability to determine whether a user is interested in clicking a button or is just looking at the button. The time for which a user needs to gaze at a particular button before it is considered as a click action is called the dwell time. In this paper, we explore intelligent adjustment of dwell times, where mouse click events on the buttons of a given application are emulated with user gaze. A constant dwell-time for all buttons and for all users may not provide an efficient and intuitive interface. We thereby propose a model to dynamically adjust dwell-time values used to emulate user mouse click events, exploiting the user’s experience with different portions of a given application. The adjustment happens at a per-user, per-button granularity, as a function of the user’s (a) prior usage experience of the given button within the application and (b) Midas touch characteristics for the given button. We propose OptiDwell, inspired by the action-value method based solutions to the Multi-Armed Bandits problem, for dwell click time adaptation. We experiment OptiDwell using an interactive TV channel browsing interface application, constituting of a mix of text and image buttons, over 10 computer-savvy users generating over 9000 click tasks. We observe significant improvement of user comfort level over the sessions, quantified by (a) improved (reduced) dwell times and (b) reduced number of Midas touches in spite of faster dwell-clicks, as high as 10-fold reduction in the best case. Our work is useful for creating an interface, with accurate, fast and comfortable dwell-clicks for each interface element (e.g., buttons), and each user.
---

Every project has a beautiful feature showcase page.
It's easy to include images in a flexible 3-column grid format.
Make your photos 1/3, 2/3, or full width.

To give your project a background in the portfolio page, just add the img tag to the front matter like so:

    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/1.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/3.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/5.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/5.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal it's glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/6.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/11.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/" target="_blank">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/6.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/11.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
```
