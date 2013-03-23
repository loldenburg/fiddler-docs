---
title: Add Rules to Fiddler
slug: AddRules
tags: Extend Fiddler, FiddlerScript, Extension, CustomRules.js, JavaScript, Customize Rules
publish: true
ordinal: 13
---

Add Rules to Fiddler
====================

Customize Rules
---------------

To add custom columns to the Fiddler UI, modify requests or responses, test application performance, and a variety of other custom tasks, add rules to Fiddler's JScript.NET CustomRules.js file in **FiddlerScript**.

1. Click **Rules > Customize Rules...**.

2. Enter FiddlerScript code inside the appropriate function.

3. Save the file.

Fiddler will automatically reload the rules.

Use Additional .NET Assemblies
------------------------------

To use additional .NET assemblies in your script:

1. Click **Tools > Fiddler Options**.

2. Click the **Extensions** tab.

3. Edit the **References** list.

4. Either:

 + Register the assembly in the GAC; or

 + Copy the assembly to the folder that contains **Fiddler.exe**.

To use the new assembly's functions without fully-qualifying them, update the **#import** clause at the top of the script.

Change the JScript Editor Launched from the **Rules** Menu
----------------------------------------------------------

1. Click **Tools > Fiddler Options**.

2. Edit the **Editor** string.

Restore Default Rules
---------------------

1. Delete the **CustomRules.js** file in **~/Documents/Fiddler2/Scripts**.

2. Restart Fiddler.

Note: Fiddler's default rules are stored in **~/Program Files/Fiddler2/Scripts/SampleRules.js**.

See Also
--------

[FiddlerScript Editor][1]

[1]: http://fiddler2.com/add-ons