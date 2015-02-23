# Product Patches for PC-lint and FlexeLint
This repository contains patches for [Gimpel Software](http://www.gimpel.com)'s PC-lint and FlexeLint.

## Applying PC-lint Patches

To determine your current patch level invoke the PC-lint program with no arguments, as in: 

<pre>
    <b>lin</b>
</pre>

or

<pre>
    <b>lint-nt -v</b>
</pre>

You will get a banner line that looks something like: 
  `PC-lint for C/C++ (NT) Ver. 9.00a, Copyright Gimpel Software 1985-2008`

From this you deduce that the patch level is '**a**' as this is the letter following "**9.00**". To update to, say, level '**c**' you would download the following files

<pre>
    lpatch.exe
    l9-a-b.lp
    l9-b-c.lp 
</pre>

With these three files in your lint directory, you would issue the commands:

<pre>
    <b>lpatch l9-a-b.lp</b>
    <b>lpatch l9-b-c.lp</b>
</pre>

You may run `lpatch` from a Windows command prompt with no arguments to get usage information. 
PC-lint patches will update only `lint-nt.exe` (the Windows executable).  They will **not** affect your configuration files.

## Applying FlexeLint Patches

To determine your current patch level invoke the FlexeLint program with no arguments. 

The file fpatch.c is used to apply the patches to the FlexeLint source modules.  Compilation and usage instructions are contained within fpatch.c 

To get fpatch.c send an email to sales@gimpel.com and please include your FlexeLint serial number and contact information (name, company, address, phone).  If we have your registration information and a signed license agreement on file, we will email you fpatch.c
'
