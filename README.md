# rice-mapping 
## Introduction
Mapping rice paddies is difficult because regions ideal for this crop are also covered by clouds. Synthetic aperture radar sensors penetrate the clouds. Developing statistic probablities from this sensor is our method for large-scale rice paddy classification.

### Requirements
If using conda, run the following commands.

```conda create -n rice-stats python=3.7```

```conda install ipykernel```

```pip install "descarteslabs[complete]"```


### First run the notebook “img_stat_product_creation.ipynb”

* Check product ID for new imagery: Make sure you delete duplicate products from existing demonstrations or modify the product ID hard-coded. 

* Run the code in sequence, substituting any year after 2014 (The Sentinel-1)

Script: 
”Adding a new product is a two step process. First you have to insert the product ID in our database, then you have to give the product information about what bands to expect. In this case, we are generating 30 statistical bands based on the VV & VH SAR bands for rice classification.”
Once that Notebook completes, You can see an empty product created in the "Your Products" section of our Catalog interface https://catalog.descarteslabs.com/?/

### Next, run the "run_stats.ipynb"
* Check the `product_id` matches your id from the previous notebook
* Run the blocks in sequence, modfiying the country if desired
* Open our monitor interface and watch the tasks advance, demonstrating features
* Open the Catalog entry for the rice stats scenes and open the resulting tiles in Viewer 
