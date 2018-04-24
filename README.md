# ScriptAssistant v0.2

By Michel Clasquin-Johnson

Public Domain Software 2015

Written for Haiku in yab, using the Yabadabbadoo IDE

So you write a lot of shell scripts, or you just like hacking on the Terminal. And you know how to get to the built-in help for each command:

    command --help

Except that some commands will only respond to -h rather than --help. And a few require you to type the command by itself, with no parameters at all. And now the help is displayed in the Terminal you were working in, so you need to open another one to continue working, and you lose your command history when you do that ...

Enter ScriptAssistant. This little app lets you select a command and throw up a window (up to 12 of them at a time) containing that command's built-in help.

ScriptAssistant requires yab to be installed. You might have it on your system alreadyand if not, the packaging system should have organised it for you.

ScriptAssistant has two modes. Normal mode contains the commands you are most likely to need while scripting: no programming or networking stuff, and .zip as the only kind of compression. Pro Mode contains absolutely everything I could find on a regulation Haiku setup that I could coax to spit out some help. This is the collection that will keep growing in future updates. Of course, any command will only work if that file is actually installed on your system. For example, I might add commands from the package Ghostscript to the database, but if you do not have Ghostscript installed, that will just display an error. The reason for this is that ScriptAssistant does not store the help data: it actually runs the command and captures the result for display. This way, the help you get is always the latest version.

I just know most of you are going to be macho and work in Pro mode all the time. Fine, but it might be a little slower and take up more screen space.

But you've added stuff since you installed Haiku, stuff I haven't gotten around to adding yet. No problem. Type the name of the command (don't bother typing the --help parameter) in the textbox at the bottom and click on TRY. ScriptAssistant will attempt to run the command with the --help parameter and capture and display the results. This can be dangerous: if the command you are investigating is interactive (e.g. a shell) and does not recognise the --help parameter, it could hang ScriptAssistant. If this happens, just wait 5 seconds and you should be back in business.

I wrote this program for my own amusement and It is now feature-complete as far as I am concerned. But please send bug reports. I could also use a nice icon.

ScriptAssistant is Public Domain software. Which means "go ahead and build a software empire on this, just don't bug me about it".  :-)

A version of ScriptAssistant is also incorporated in my alternative yab IDE, Yabbadabbadoo. Nothing terrible should happen if you run both versions.

Get it here: https://github.com/clasqm/ScriptAssistant
