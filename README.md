# meteor-issue-8441

Reproduction for https://github.com/meteor/meteor/issues/8441.

## Steps

1. `git clone https://github.com/hwillson/meteor-issue-8441.git`
2. `cd meteor-issue-8441; meteor`
3. Watch the server console; the app can't be started as the `/private/dir2` symlink to `/private/dir1` is causing problems.
4. Remove the `/private/dir2` symlink; the app starts properly. 

