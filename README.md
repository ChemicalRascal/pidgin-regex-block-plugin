pidgin-regex-block-plugin
==========================

This is a Pidgin IM client plugin that allows you to specify a regex pattern such that if the pattern is match in any open conversation window or chat room window, the message will be blocked (or, in libpurple lingo, canceled).

This plugin is of use if you want to block messages that are known in advance to match regex patterns.

To install it, just copy: PidginNotifyIfMessageMatch.pl to your ~/.purple/plugins/ directory (%AppData%\.purple\plugins on Windows). Then, after restarting Pidgin, via Tools->Plugins, find "Block Message Match Plugin" and enable it.

On Windows, you will need to install a specific version of Perl to make Pidgin recognise that you have Perl installed, as alas if you do not, Perl plugins will be disabled. For Pidgin 2.10.12 and newer (as of Pidgin 2.11.0, at least), this is Perl 5.20.*, in 32-bit. [See developer.pidgin.im for more information.](https://developer.pidgin.im/wiki/Scripting%20and%20Plugins#WhydoesntmyPerlpluginshowupinthePluginsdialog)

[Just want to end the suffering and get the right version of Perl? Strawberry Perl 5.20.3.3 worked for the author.](http://strawberryperl.com/releases.html) Notably, he didn't have Strawberry Perl, of any version, installed already, but did have another distribution installed, and they seemed to co-exist comfortably maybe?

The author does not know if there is a way to make Perl work for Pidgin Portable, but he suspects not. Don't blame him, blame the Pidgin developers.

Configuration accepts a single perl regular expression. Patches expanding this to a user-configurable list of regular expressions would be most welcome.