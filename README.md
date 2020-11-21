# Zilu Su
# Synthetic Training Data Generation for Object Co-Segmentation


## Image Synthesis Methods
### Method_1.ipynb
Obtain foreground instances via COCO annotations.       
Then augment foregrounds, genearate new masks and paste foregrounds onto backgrounds.      

INPUT:
    instances_val2017.json - COCO annotation information         
    background - Indoor Scene dataset          
OUTPUT:
    mask and image        


### Method_2.ipynb
Extract foreground instances via Mask R-CNN and GrabCut.           

INPUT:
    foreground resource, extracted foreground, background         
OUTPUT:
    mask and image          


### Method_3.ipynb
Use images without background as foregrounds directly.           
    
INPUT:
    foreground and background           
OUTPUT:
    mask and image            
  
  


## Data Processing
### data_real.ipynb 
Process COCO dataset with required information for JSON file.         
  
### data_synthetic.ipynb
Composite images via the first method with COCO annotations.           
Generate corresponding JSON file for mask segmentation information.             

### data_train_test.ipynb
Copy data from 10 categories to traning and testing datasets.              
 



## baseline_data.zip
Train: 216 real images with corresponding JSON files(10 categories)            
Test: 50 real images (5 images for each category)              

## mixed_data.zip
Train: 216 real images (same as baseline) + 998 synthetic images                 
Test: same as baseline            




## baseline.ipynb
Baseline data training and testing          
mean Average Precision:  0.58                   

## synthesis_evaluation.ipynb
Mixed data training and testing              
mean Average Precision:  0.82               




# Thank You for Mentoring
