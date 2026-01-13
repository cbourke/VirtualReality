
**Compiler errors are not highlighted in the VS Code editor**

Or automatic code completion may not be working.  You need to tell Unity to use
Visual Studio as its script editor.  In Unity:

`edit > preferences > external tools > external script editor > Visual Studio`

close and reopen Visual Studio.  If prompted, click `no` on the firewall prompt.

**In GitHub desktop you get a message like "LF will be replaced with CRLF" and it doesn't let you commit**

This happens because you made the *parent *folder/directory of your Unity
project into the git repo instead of the Unity project's folder.  Consequently,
the `.gitignore` file is not ignoring what it should be (and a bunch of
generated code/files are wanting to be committed).

The *quick* fix is to copy your `.gitignore` file into your Unity project
subfolder so it ignores everything with respect to that directory.
The *correct* fix is that next time you create a repo, make sure it is
done in the Unity project folder.  Generally there should be 1 Unity
project to 1 repo (otherwise you're gonna run out of room quick).

**GitHub Unity Plugin Alternative*

Here is an alternative to using the GitHub Unity plugin (this replaces section 3.1.1 in the Module 1.0 handout):

1. Create Unity project
2. Create github repo, give it the Unity .gitignore, and clone it locally
3. Close Unity
4. Move all contents of the Unity project folder to the repo folder. Push changes
5. Open Unity Hub, remove the old project and add the repo folder as an existing Unity project

Section 3.1.2 is written assuming that you use the GitHub Unity Plugin; if you choose not to use the plugin, you should use the github desktop client instead; it should be straightforward on how to COMMIT (with a commit message) changes and PUSH them to a remote repo and (when your partner makes changes) to PULL those changes (it should detect them automatically) all through the github desktop client.  If not, we can find some more instructions or when it comes to that step, tell us and we'll walk you through out.
 - Section 4.1.1 (where you add a collaborator to your repo) is done using the github desktop client, so no changes are needed there
