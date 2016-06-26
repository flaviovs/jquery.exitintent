jQuery Exit Intent Plugin
=========================

The jQuery Exit Intent plugin try to anticipate when the user is about
to leave the current page, and fire an event when it thinks they are
doing so. You can react to this event to display modal dialogues,
change page text, etc., to try to grab user's attention and
(hopefully) made them change their minds.


Requirements
------------

1. jQuery >= 1.4


Installation
------------

1. Download the plugin

2. Include the following line *after* jQuery:

        <script src="jquery.exitintent.min.js"></script>

   NB: adjust the path as necessary

3. Enable the plugin in your site:

        $.exitIntent('enable');

4. Listen to the `exitintent` event, and act accordingly:

        $(document).on('exitintent',
            function() {
                console.log('Oops... trying to leave the page');
            });


FAQ
---

1. How do I display a modal popup when the user is trying to leave my
page?

   This plugin only deals with detecting when the user is leaving the
   page, and triggering the `exitintent` event. It's up to you do
   define *what* you want to do when the user is leaving. For example,
   if you want to display a modal dialog, you may use your preferred
   jQuery modal plugin to display the modal.


Legal
-----
Copyright (C) 2016 Flávio Veloso

This plugin is released under the terms of the MIT license. See the
LICENSE file for more details.

If you think you found a bug in this plugin, please visit
https://github.com/flaviovs/jquery.exitintent/issues and open a new
issue.
