=== Paid Memberships Pro - Infusionsoft Add On ===
Contributors: strangerstudios
Tags: pmpro, paid memberships pro, infusionsoft, email marketing
Requires at least: 4
Tested up to: 5.4.1
Stable tag: 1.4

Sync your WordPress users and members with Infusionsoft groups and tags.

== Description ==

This plugin has been replaced by the free Keap Integration for Paid Memberships Pro.

Please refer to the new [Keap Integration Add On documentation](https://www.paidmembershipspro.com/add-ons/keap-integration/) to access the free plugin download and get steps to set up the plugin.

== Installation ==

THIS PLUGIN IS NO LONGER BEING MAINTAINED. WE DO NOT RECOMMEND USING THIS PLUGIN ANYMORE.

== Frequently Asked Questions ==

= I found a bug in the plugin. =

Please post it in the issues section of GitHub and we'll fix it as soon as we can. Thanks for helping. https://github.com/strangerstudios/pmpro-infusionsoft/issues

= I need help installing, configuring, or customizing the plugin. =

Please visit our premium support site at http://www.paidmembershipspro.com for more documentation and our support forums.

== Screenshots ==

1. Settings screen to add Infusionsoft Username/ID and API Key; Assign All Users Tags and per-Membership Level Tags.

== Changelog ==
= 1.4 =
* BUG FIX/ENHANCEMENT: If you have more than 1000 tags/groups, we will import them all into the settings page. We are using the select2 library to make it easier to search and add tags on those pages.
* BUG: Checking if iSDK is already loaded before loading again to prevent conflicts with other plugins loading the SDK. Issues may still persist if the plugins load different versions of the SDK.

= 1.3.1 =
* BUG: Fixed issue where membership level tags were being replaced when a user updated their profile. (Thanks, Scott Slone)

= 1.3 =
* IMPORTANT UPGRADE. Removed some debugging code that could lock up websites when the plugin was activated. Please upgrade.

= 1.2.1 =
* Fixed warnigns and bug in the test connection code.
* Made sure errors show up on settings page if the connection to Infusionsoft can't be made.

= 1.2 =
* Now testing API connection when plugin initializes. If it fails, error will be displayed in the General Settings section.

= 1.1 =
* Fixed issue with updating contact info if the user changed their email address. (Thanks, Matt Cherry)

= 1.0 =
* Released to the WordPress repository.

= .6 =
* Now getting tags from Infusionsoft and showing them in a multiselect box on the options page.
* When a user changes levels or cancels, the plugin will now remove tags based on the level they are changing from.

= .5 =
* Updates contact information in Infusionsoft if it is updated on the WP side. (Thanks, Matt Cherry.)

= .4.1 =
* Fixed dup check that was keeping contacts from being added.
* Now updating user info if someone checks out again. At checkout a contact with no name/etc is added, then when pmpro_after_checkout fires, the contact is updated with the full user data.

= .4 =
* Added extra call to update contact at checkout to give PMPro time to update user meta.
* Added pmpro_infusionsoft_addcon_fields filter to update additional fields when updating contacts.
* Fixed bug in preg_replace for duplicate check.

= .3 =
* Including the xmlrpc.inc file from Infusionsoft for older PHP versions.
* The Infusionsoft username/id is now a settings field vs being hard coded into the plugin files.
* Removed the krumo require.

= .2 =
* Added readme. This version is actually working and pushing users to Infusionsoft.
