PROJECT 1: COPY DATA PIPELINE TO COPY FILES FROM SOURCE FOLDER TO THE DESTINATION IN MICROSOFT FABRIC

Step 1: Create a workspace with the desired name for the project
<img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/8bae17ae-8201-450b-b189-7e18b337584b" />

Step 2: Create a Lakehouse in the workspace
<img width="788" height="222" alt="image" src="https://github.com/user-attachments/assets/76535aa4-a21c-40d6-bef9-9522069d30b6" />

Step 3: Navigate to the specific Lakehouse and then create two subfolders source and destination and add the file(in my case in csv) to the source folder and then create a destination folder
as shown below
<img width="389" height="431" alt="image" src="https://github.com/user-attachments/assets/105d7dd6-c82b-4d03-ad2d-9741429bc7ad" />

Step 4: Now create a new pipeline named CopyData Activity in your desired lakehouse
Create a copy data activity with the Source and the Destinations customized accordingly

<img width="1530" height="953" alt="image" src="https://github.com/user-attachments/assets/3cdef80e-7863-49d7-b4d2-721281cd2a1a" />

Source Details:
================================================
<img width="1602" height="415" alt="image" src="https://github.com/user-attachments/assets/9d272a0f-3ac8-4712-8f05-38573ba4c87d" />

Destination Details in the Pipeline:
==========================================================
<img width="1524" height="335" alt="image" src="https://github.com/user-attachments/assets/6d0e1f00-9e45-4cc9-92aa-a6703a1e0414" />

Now after the destination is defined, give the name of the file and validate the pipeline

<img width="506" height="754" alt="image" src="https://github.com/user-attachments/assets/40db0a67-70fd-4e39-a9c1-fc412d10836e" />

Now run the pipeline using Save and Run with the Data pipeline

<img width="673" height="210" alt="image" src="https://github.com/user-attachments/assets/797de532-66d3-4ede-aad7-db09f0956fcf" />

Check the activity runs, It shows as succeeded
<img width="1275" height="411" alt="image" src="https://github.com/user-attachments/assets/cd4e7429-3d8f-4499-b41f-869df4740548" />

Once the pipeline is succeeded, refresh the folder in the Data Lakehouse and it will show the file with the contents transferred from source to Destination

Destination Folder with the copied File
<img width="1425" height="326" alt="image" src="https://github.com/user-attachments/assets/295afda2-f474-4d8a-97a6-1ee6d0cb124d" />

This Copy Data Activity is the crucial step when we are trying to copy the data from the source folder to the Destination folder in the Lakehouse


