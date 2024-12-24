**To create ad-hoc images:**

1. Create a new branch matching the tag of the image you want to push to GCR
2. Copy the Docker file and CI file to the branch. The CI file can be used as is without any changes
3. Any commit to the branch will build and push the image to the GCR with the following tags:

   a. gcr.io/kodekloud/customimage:<branch_name></br>
   
   b. gcr.io/kodekloud/customimage:<branch_name_sha> 