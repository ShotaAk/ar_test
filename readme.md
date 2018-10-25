# ar_track_alvarのバグチェック

## 起動

```zsh
$ roslaunch ar_test ar_test.launch tf:=true

$ roslaunch ar_test ar_test.launch tf:=false
```

## エラーが出る

```zsh
$ roslaunch ar_test ar_test.launch tf:=true

[ERROR] [1540440881.212420110]: "camera" passed to lookupTransform argument source_frame does not exist. 
[ERROR] [1540440881.212420110]: "camera" passed to lookupTransform argument source_frame does not exist. 
[ERROR] [1540440881.212420110]: "camera" passed to lookupTransform argument source_frame does not exist. 



$ roslaunch ar_test ar_test.launch tf:=false

[ERROR] [1540441612.739433484]: "head_camera" passed to lookupTransform argument target_frame does not exist. 
[ERROR] [1540441612.739433484]: "head_camera" passed to lookupTransform argument target_frame does not exist. 
[ERROR] [1540441612.739433484]: "head_camera" passed to lookupTransform argument target_frame does not exist. 
```

