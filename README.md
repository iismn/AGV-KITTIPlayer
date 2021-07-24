![header](https://capsule-render.vercel.app/api?type=rect&color=timeGradient&text=SEMANTIC%20KITTI%20BAG&fontSize=20)

## <div align=left>:heavy_plus_sign:REPO INFO</div>  
- KAIST IRiS Lab. Autonomous Vehicle "PHAROS" 
- Semantic KITTI ROS BAG (with GPS/IMU for LIO-SAM)

## <div align=left>:heavy_plus_sign:REPO CONFIG</div>  
### kitti2bag
* File Directory Consist with
```bash
├── 2011_09_26
│   ├── 2011_09_26_synced
│   └── 2011_09_26_extract
├── kitti2bag.py
└── util.py
``` 



## <div align=left>:heavy_plus_sign:REPO USE</div> 
```bash
wget https://s3.eu-central-1.amazonaws.com/avg-kitti/raw_data/2011_09_26_drive_0084/2011_09_26_drive_0084_sync.zip
wget https://s3.eu-central-1.amazonaws.com/avg-kitti/raw_data/2011_09_26_drive_0084/2011_09_26_drive_0084_extract.zip
wget https://s3.eu-central-1.amazonaws.com/avg-kitti/raw_data/2011_09_26_calib.zip
unzip 2011_09_26_drive_0084_sync.zip
unzip 2011_09_26_drive_0084_extract.zip
unzip 2011_09_26_calib.zip
python kitti2bag.py -t 2011_09_26 -r 0084 raw_synced .
```

## <div align=left>:heavy_plus_sign:ADD INFO</div>
#### SEMANTIC KITTI for LIO-SAM
- Only 2011_09_30 work
- Odometry 00~07 Not Tested
