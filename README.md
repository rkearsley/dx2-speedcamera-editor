# dx2-speedcamera-editor
It's a windows application to re-write the Thinkware F770 dash cam's speed camera alert list.

## Thinkware F770
This dash cam is quite a high end one, and has a gps receiver in it, so it has the really useful (but also potentially annoying) feature which gives spoken warnings when approaching a speed camera

## The problem
While the alerts works well for fixed and red-light cameras, the vast majority of the alerts are for mobile speed cameras. This is particularly annoying while driving on certain sections of motorway where the alerts can be every few seconds. They can't be disabled through a user option, and are only silenced when driving 10% under the limit which sadly is not very useful as most of us will likely drive at the limit. The dx2 file is a proprietary binary file, which stops us easily editing it (e.g in a text editor) and removing the mobile entries. Others have noticed this problem too https://dashcamtalk.com/forum/threads/annoying-speed-camera-zone-announcement.27289

## The solution
I have created this application which opens the dx2 files and can interpret the binary format somewhat. As I don't have any specification on the file format, I wasn't able to decipher many of the data fields. However, it can remove entries and also edit the speed limits which is all we really need. The possible options are:
- remove all cameras of a certain type (e.g. mobile speed camera type)
- change the speed limit of a certain type to be +10% or higher (e.g set 80 mph on a UK motorway instead of 70)
- a third option I discovered was to change the camera type e.g. change mobile to red-light with disable the spoken alert but play the chime sound instead

