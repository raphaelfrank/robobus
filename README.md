# RoboBus: A Diverse and Cross-Border Public Transport Dataset
Academic datasets are an important source of information to validate and benchmark novel research concepts. In this paper we present RoboBus, a dataset recorded with a commercial bus on a cross-border public transport route between Luxembourg and France. The dataset contains approximately 8 hours of driving data divided into 15 trips that have been recorded over 4 days. It includes about 1.7 million anonymized images capturedby two road-facing cameras, GNSS traces, data from a 9-axis IMU, and information directly retrieved from the CAN interface of the vehicle including speed, steering angle and position of the accelerator/brake pedals.

## Dataset

### Data Format

[CSV_FILE]
|
+--[TYPE]
|
+--[TIME (ms)]
|
+--[CAN_DATA (type 1)]
|	 |
|  +—[VEHICLE_SPEED (km/h)]
+--[CAN_DATA (type 2)]
|	 |
|  +—[ACC_PEDAL_POSITION]
+--[CAN_DATA (type 3)]
|	 |
|  +—[BRK_PEDAL_POSITION]
+--[CAN_DATA (type 4)]
|	 |
|  +—[STE_WHEEL_ANGLE]
+--[IMU_DATA (type 50, 51 and 52)]
|	 |
|  +—[ACC/MAG/GYR X]
|  +—[ACC/MAG/GYR Y]
|  +—[ACC/MAG/GYR Z]
+--[GNSS_DATA (type 100)]
|	 |
|  +—[TIMESTAMP]
|  +—[LATITUDE]
|  +—[LONGITUDE]
|  +—[ALTITUDE]
+--[CAMERA_INFO (type 201 and 202 )]
|	 |
|  +—[PATH_TO_IMAGE]

### Example Images
![alt text](https://github.com/raphaelfrank/robobus/blob/main/sample_images.png?raw=true)

## Downloads
The total dataset is ~67GB and can be downloaded [here](https://dropit.uni.lu/invitations?share=c73d2e4064ec02181159).

## Acknowledments
This work has been financially supported by the [EU INTERREG GR Terminal project](https://terminal-interreg.eu/en/a-lighthouse-project-on-mobility-in-the-greater-region-2/). The authors would also like to thank Voyages Emile Weber Luxembourg for their support and for granting us access to their bus.
