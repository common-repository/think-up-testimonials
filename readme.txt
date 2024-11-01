=== Plugin Name ===
Contributors: cipes
Donate link: n/a
Tags: testimonials, rotator, responsive, easy, text widget,
Requires at least: 3.0.1
Tested up to: 4.5.3
Stable tag: 1.3
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

A simple to use responsive testimonials rotator that uses WP's native text widgets and a sidebar.

== Description ==
Think Up Testimonials rotator uses WP's native text widgets and a plugin created sidebar. Put your testimonials into individual
text widgets with the following markup.

<code><h3>Your nice quote from someone saying how great your or business are.</h3><h2>~ Andy Johnson</h2></code>

Place the text widget into the sidebar called 'Think Up Testimonials'. To output the testimonial rotator on the front end, insert
the function `thinkup_testimonials()`` into your theme template files where you want the rotator to appear.  You can also control the
time for each slide and if you want the rotator to autoplay or not through the callback function.

To create a slider within your template that rotates every 9 secs use the code <code>thinkup_testimonials(9000);</code>

To stop the default auto-rotate of the plugin, add the `false` parameter to the callback function like this <code> thinkup_testimonials(9000, false); </code>


== Installation ==

1. Upload the `thinkup-testimonials` folder to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Go to the widgets page and place a normal text widget in the 'Think Up Testimonials' sidebar and add a testimonial using this mark up <code><h3>Testimonial text here</h3><h2>~ Author</h2></code>
4. Repeat step 3 as needed.
5. Place `thinkup_testimonials();` in your templates to output the rotator
6. If you want to control the timing of the rotator, include the time (in milliseconds) within the callback function. ie: `thinkup_testimonials(9000);` creates a slider with a 9 sec delay.
7. If you want to stop the default auto-rotate feature, just add a second parameter 'false' to the callback function like so `thinkup_testimonials(9000, false);`

== Frequently Asked Questions ==

= How can you change the size of the testimonial or author text? =

Simply use your style.css of your theme to overwrite the plugin styles. Use the CSS selector #thinkup-testimonials h3 {...}
for the testimonial text and #thinkup-testimonials h2 {...} for the author text.

= How can you change the delay between testimonials? =

You are able to set the delay time between testimonials using the callback function.  Place the delay time (in milliseconds) with the brackets of the
the callback function. ie: thinkup_testimonials(9000); would set the time delay to 9 seconds between testimonials.

== Screenshots ==

1. A standard implementation of the Think Up Testimonials plugin with 3 testimonials.  Font styles are created by the theme.
2. The back end look at the text widgets, markup used and the Testimonials sidebar.

== Changelog ==

= 1.3 =
* Added ability to cancel auto-rotate by adding 'false' to the callback function.

= 1.2 =
* Allows user to specify delay between slides with callback function.

= 1.1.2 =
* Fixes to specificity of TUT-Flexslider CSS so plugin does not conflict with other independent flexslider instances

= 1.1 =
* Added rotator time delay setting thinkup-testimonials() callback function

= 1.0 =
* First version released to the wild
