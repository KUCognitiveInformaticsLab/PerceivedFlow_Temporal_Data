# PerceivedFlow_Temporal_Data

The data from the "Temporal Dynamics of Perceived Motion Flow in Naturalistic Movie Sequences" is contained in this folder.

Dataset S1 (Raw response data). The motion vectors of raw response are supplied in Temporal_Response.mat 

    7D matrices: 2 (uv components) x 4 (probed locations) x 4 (flip conditions in image coordinates) x 2 (play directions) x 5 (probe timing) x 5 (movies) x 4 (participants).

Dataset S2 (Ground truth data). The motion vectors of ground truth are supplied in Temporal_GT.mat 
    
    6D matrices: 2 (uv components) x 4 (probed locations) x 2 (play directions) x 5 (probe timing) x 5 (movies) x 15 (frames).


Dataset S3 (FlowNet 2.0). The predicted motion vectors of FlowNet 2.0 are supplied in Temporal_FN2.mat 
   
    6D matrices: 2 (uv components) x 4 (probed locations) x 2 (play directions) x 5 (probe timing) x 5 (movies) x 14 (frames).


Dataset S4 (Fitting functions with all Observers). The predicted motion vectors of four fitting functions with all observers are supplied in Temporal_AllObservers.mat 

    6D matrices: 2 (uv components) x 4 (probed locations) x 2 (play directions) x 5 (probe timing) x 5 (movies) x 4 (models).



Dataset S5 (Fitting functions by Observers). The predicted motion vectors of four fitting functions by observers are supplied in Temporal_ByObservers.mat 
    
    7D matrices: 2 (uv components) x 4 (probed locations) x 2 (play directions) x 5 (probe timing) x 5 (movies) x 4 (participants' prediction) x 4 (models).
    
In Datasets S2 and S3, the 8th frame is the probed target frame

In Datasets S4 and S5, the four models:

  a. L2 regularized regression (ground truth inputs)

  b. L2 regularized regression (FlowNet 2.0 inputs)
 
  c. Gaussian fitting (ground truth inputs)
  
  d. Gaussian fitting (FlowNet 2.0 inputs)
