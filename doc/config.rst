Configuration Parameters
------------------------
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| Name                                | Command Flags                 | Type  | Default       | Comment                                                                     |
+=====================================+===============================+=======+===============+=============================================================================+
| ``log_time``                        | | ``--log-time``              | bool  | ``false``     | Show date and time in logs                                                  |
|                                     | | ``--no-log-time``           |       |               |                                                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``cleanup``                         | | ``--cleanup``               | bool  | ``true``      | Cleanup cache or temporary files after conversion                           |
|                                     | | ``--no-cleanup``            |       |               |                                                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``auto_sqlite``                     |                               | bool  | ``true``      | Auto-enable ``--sqlite`` to limit RAM usage when direct                     |
|                                     |                               |       |               | mode is not possible. Can override with ``--no-sqlite``                     |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``enable_alts``                     | | ``--alts``                  | bool  | ``true``      | Enable alternates                                                           |
|                                     | | ``--no-alts``               |       |               |                                                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``skip_resources``                  | ``--skip-resources``          | bool  | ``false``     | Skip resources (images, audio, css, etc)                                    |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``save_info_json``                  | ``--info``                    | bool  | ``false``     | Save .info file alongside output file(s)                                    |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``lower``                           | | ``--lower``                 | bool  | ``false``     | Lowercase word(s)                                                           |
|                                     | | ``--no-lower``              |       |               |                                                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``utf8_check``                      | | ``--utf8-check``            | bool  | ``false``     | Fix Unicode in word(s) and definition                                       |
|                                     | | ``--no-utf8-check``         |       |               |                                                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``rtl``                             | ``--rtl``                     | bool  | ``false``     | Make definition right-to-left                                               |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``remove_html``                     | ``--remove-html``             | str   | ``""``        | Remove given comma-separated HTML tags (not their contents) from definition |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``remove_html_all``                 | ``--remove-html-all``         | bool  | ``false``     | Remove all HTML tags (not their contents) from definition                   |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``normalize_html``                  | ``--normalize-html``          | bool  | ``false``     | Normalize HTML tags in definition (WIP)                                     |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``skip_duplicate_headword``         | ``--skip-duplicate-headword`` | bool  | ``false``     | Skip entries with a duplicate headword                                      |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``trim_arabic_diacritics``          | ``--trim-arabic-diacritics``  | bool  | ``false``     | Trim Arabic diacritics from headword                                        |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``unescape_word_links``             | ``--unescape-word-links``     | bool  | ``false``     | Unescape Word Links                                                         |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``color.enable.cmd.unix``           | ``--no-color``                | bool  | ``true``      | Enable colors in Linux/Unix command line                                    |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``color.enable.cmd.windows``        | ``--no-color``                | bool  | ``false``     | Enable colors in Windows command line                                       |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``color.cmd.critical``              |                               | int   | ``196``       | | Color code for critical errors in command line                            |
|                                     |                               |       | |image0|      | | See `term-colors.md <./term-colors.md/>`_                                 |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``color.cmd.error``                 |                               | int   | ``1``         | | Color code for errors in command line                                     |
|                                     |                               |       | |image1|      | | See `term-colors.md <./term-colors.md/>`_                                 |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``color.cmd.warning``               |                               | int   | ``208``       | | Color code for warnings in command line                                   |
|                                     |                               |       | |image2|      | | See `term-colors.md <./term-colors.md/>`_                                 |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``cmdi.prompt.indent.str``          |                               | str   | ``">"``       |                                                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``cmdi.prompt.indent.color``        |                               | int   | ``2``         |                                                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``cmdi.prompt.msg.color``           |                               | int   | ``-1``        |                                                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``cmdi.msg.color``                  |                               | int   | ``-1``        |                                                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``ui_autoSetFormat``                |                               | bool  | ``true``      |                                                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``tk.progressbar.color.fill``       |                               | str   | ``"blue"``    | Tkinter: progressbar fill color                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``tk.progressbar.color.background`` |                               | str   | ``"gray"``    | Tkinter: progressbar background color                                       |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``tk.progressbar.color.text``       |                               | str   | ``"yellow"``  | Tkinter: progressbar text color                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``tk.progressbar.font``             |                               | str   | ``"Sans"``    | Tkinter: progressbar text font. Example: "Sans", "Sans 15"                  |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``reverse_matchWord``               |                               | bool  | ``true``      |                                                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``reverse_showRel``                 |                               | str   | ``"Percent"`` |                                                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``reverse_saveStep``                |                               | int   | ``1000``      |                                                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``reverse_minRel``                  |                               | float | ``0.3``       |                                                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``reverse_maxNum``                  |                               | int   | ``-1``        |                                                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+
| ``reverse_includeDefs``             |                               | bool  | ``false``     |                                                                             |
+-------------------------------------+-------------------------------+-------+---------------+-----------------------------------------------------------------------------+

Configuration Files
-------------------

The default configuration values are stored in `config.json <./../config.json/>`_
file in source/installation directory.

The user configuration file - if exists - will override default configuration
values. The location of this file depends on the operating system:

- Linux or BSD: ``~/.pyglossary/config.json``
- Mac: ``~/Library/Preferences/PyGlossary/config.json``
- Windows: ``C:\Users\USERNAME\AppData\Roaming\PyGlossary\config.json``

Using as library
----------------

When you use PyGlossary as a library, neither of ``config.json`` files are
loaded. So if you want to change the config, you should set ``glos.config``
property (which you can do only once for each instance of ``Glossary``).
For example:

.. code:: python

	glos = Glossary()
	glos.config = {
		"lower": True,
	}


.. |image0| image:: https://via.placeholder.com/20/ff0000/000000?text=+
.. |image1| image:: https://via.placeholder.com/20/aa0000/000000?text=+
.. |image2| image:: https://via.placeholder.com/20/ff8700/000000?text=+