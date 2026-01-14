# OpenPose2tab
Read all OpenPose json files and create single tab separated file for pose_keypoints_2d for single person

The script uses some Windows commands: dir and mkdir. These can be replaced with e.g. linux commands ls and mkdir.
The script requires the name of a root folder and the name of a subfolder of the root folder, for example:

    FinalDataset
        20220916

The script searches for a folder that contains files with the extension '.json' under the subfolder. These files can be in the subfolder itself.
The output is in a folder keypoints.tab and would be called keypoints.tab/20220916.tab

usage:

    bracmat "get$\"jsn2tab.bra\"" <root> <subfolder>

Without the last two arguments, their values are taken from the lines

    (Root=FinalDataset)
    (meetings=20220916)

in the script.

The Bracmat interpreter can be obtained from https://github.com/BartJongejan/Bracmat
