# Rail-defect-datasets
Collection of synthetic datasets for rail surface and geometry defect detection. This collection includes 4 datasets:

- FT100: Dataset containing 100 images with surface defects. Each image contains a random number of surface defects from a minimum of 1 to a maximum of 3. The variation of the dataset is low with the same POV and lighting conditions on every image.

- Korea1500: Dataset containing 1500 images with surface defects. Each image contains a random number of surface defects from a minimum of 1 to a maximum of 4. The variation of the dataset is higher as compared to FT100 with the POV slightly changing and images showcasing different locations with different lighting and environmental conditions.

- Swiss500: Dataset containing 500 images with surface defects. Each image contains a random number of surface defects from a minimum of 1 to a maximum of 3. This dataset showcases railtracks having different lighting conditions and rail materials as compared to FT100 and Korea1500.

- Geometry testset: This dataset consist of 100 images for geometry defect classification, where 50 of those images are anomalous and 50 are normal. The defects are randomly located along the rail and can be randomly found in the right rail, left rail or both.

Images of FT100, Korea1500 and Geometry testset showcase railtracks from Korea and were created using videos provided by Korail as a source. Images of Swiss500 showcase railtracks from Switzerland and were created using videos from youtube showing the rail environment in Switzerland.

The datasets have this naming format for the images:

ID1_ID2_list-of-defects_number-of-defects/right-left.jpg

Where, 
- ID1 and ID2 correspond to IDs given to the images inside the datasets or inside the video they where collected from.
- list-of-defects correspond to the rail defects found on the image which can be the following: RG (geometry defect), RH (rail hole), RB (broken rail), RC (rail crack) or RS (rail squat).
- number-of-defects/right-left corresponds to the number of defects found in the images in the case of surface defect detection datasets and the affected rail in the case of Geometry testset, being R the right rail, L the left rail and RL both rails.

Examples:
1_19951_RH-RS-2.jpg ---> Image of ID 1 and video frame ID 19951 containing a rail hole and a rail squat.
3_RG_R.png ---> Image of ID 3 containing a geometry defect affecting the right rail.

The datasets created for surface anomaly detection contain annotation files apart from the images. Each annotation file is a .txt file that corresponds to an image of the same dataset. The name of the .txt file is the same as the image it corresponds to but with the extension changed from .jpg to .txt. The annotations include coordinates of bounding boxes, each line of the file corresponding to a single bounding box.

The datasets can be found in the following shared folder:
https://drive.google.com/drive/folders/1kj8FCsXcyeAkrUzfpDcJYuib6dKVjJ8m?usp=drive_link

