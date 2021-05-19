# dark-mode-toggle
Neat and easy-to-use css-only dark mode toggle.

Why?
Many people prefer to view their pc / laptop / tablet / cell phone screens with light text on a dark page, rather than the more usual dark text on a light page. It would be useful to provide the user with a simple means of selecting the setting according to his preference.

How?
With the implementation of variables in css, more correctly known as custom properties, this has now become quite do-able. It is straightforward to define two sets of colors, and to switch between them as required. In fact one could even define a set of color themes and switch between them.

In the case of multiple (i.e. more than two) themes we would probably use radio buttons to make the selection. (A radio button is a means of providing multiple options, where only one may be selected at a time.) In this implementation, because there are only two options, it is preferred to use a checkbox (which is either checked or not checked), to make the selection between the two themes.

A checkbox is typically a small square with or without a tick mark in it; in this project it has been decided to hide the checkbox, and to display its (variable text!) label, formatted as a button, all in the name of being more user-friendly.

Features
The button at the top of this page toggles the theme between two states, light mode and dark mode.
The last used state is remembered by the system, and on the next visit to the page the user's choice will be re-applied. If no choice has been made, the page default is used.
Some browsers enable the user to select dark or light mode; Windows has an App dark/light mode setting. These settings are respected by the switcher and the user's choice will be applied by default. The user can still toggle back and forth thereafter.
The switcher is fully operational using only CSS, although a small javascript is used to recall the previous state and to re-apply it on a subsequent visit to the page. If javascript is not available or if it is disabled, the switcher will use the default setting.
There is not a limit on the properties that can be toggled. Note the following in this demo:
background (light grey/dark grey)
text (dark grey/light grey)
headings (blue/green)
button text ("Switch to dark mode"/"Switch to light mode")
