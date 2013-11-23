## Sudoers Workflow

First: avoid, at all costs, adding a sudo entry. Only add an entry to your sudoers file as
a last resort.

If you do need to add an entry, however, this is a great way to do it because it will check
your syntax with visudo, making sure that you do not break your sudoers file (which is 
really, really bad).

Also included is "which" command that allows you to grab the path of the command you need
to add to the sudoers file. Hence, just invoke "which <command_name>" and the path will 
be copied to your clipboard.

After that, type "addsudo" — no arguments. You'll be prompted to put in your password. Do
that to be able to edit the file. Then, there will be a dialog box that pops up. Just 
paste the command here and add any arguments that you need. If the command is valid, then
it will write a line to the file that will give the current user permissions to use that
command without a password (here, obviously is the potential security threat that makes
adding a line to the file a last resort).

The nice thing about this workflow is that it will not let you break your sudoers file. So
if you aren't familiar with the syntax but need to add an entry, then use this rather than
trying to edit it yourself.

