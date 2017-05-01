# Theme Breakpoints for Javascript

This module exposes theme-related breakpoints as
directly usable Javascript variables.

## Usage

When developing client-side Javascript applications,
you might need to know about the breakpoints your currently used theme defines.
Themes can define breakpoints <a href="https://www.drupal.org/docs/8/theming-drupal-8/working-with-breakpoints-in-drupal-8">this way</a>,
but they're not exposed automatically for client-side behaviors.

This module helps developers by exposing the breakpoints
as Javascript variables, being directly accessible via
<code>window.themeBreakpoints</code>. This object also provides a helper
function <code>getCurrentBreakpoint()</code>, which tells you the currently
matching breakpoint for the given client.

Backend developers can use the <code>theme_breakpoints_js</code>
service for conveniently receiving breakpoints defined by themes.
It already takes care about defined breakpoints by base themes and also
loads them in case a theme doesn't define breakpoints by itself.

# Installation

- This module obviously depends on Drupal core's breakpoint module.
- Install this module <a href="https://www.drupal.org/docs/8/extending-drupal-8/installing-modules">as usual</a>.
- No configuration required. Once enabled, the currently used theme's breakpoints are available as JS variables.
