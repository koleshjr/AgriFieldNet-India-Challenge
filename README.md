# Solution for AgriFieldNet India Challenge

The solution contains two notebooks:
1. `data_load.ipynb`
This notebook contains the code to load the data and create the train and test datasets. it first loads the data from the radiant earth MLHub and then creates four csv files in the current directory:
    * `tile_df.csv`
    * `tile_field_df.csv`
    * `pixel_df.csv`
    * `field_crop_df.csv`
To run this notebook you first need to install the required libraries in the file `requirements.txt`. You can do this by running the following command in the terminal:
```
pip install -r requirements.txt
```
    

2. `solution.ipynb`
This notebook contains the code for the solution. It first loads the data from the csv files created by the `data_load.ipynb` notebook. It is runned in google colab using GPU runtime. To run this notebook you first need to upload the data to the runtime. if you are using google drive you just need to change the variable `path`. 

After running this notebook you should get the `submission.csv` file in the current directory, which is the final prediction.