# Kaggle-Notebook


Official API for https://www.kaggle.com, accessible using a command line tool implemented in Python 3.



#API credentials
To use the Kaggle API, sign up for a Kaggle account at https://www.kaggle.com. Then go to the 'Account' tab of your user profile (https://www.kaggle.com/<username>/account) and select 'Create API Token'. This will trigger the download of kaggle.json, a file containing your API credentials. Place this file in the location ~/.kaggle/kaggle.json (on Windows in the location C:\Users\<Windows-username>\.kaggle\kaggle.json - you can check the exact location, sans drive, with echo %HOMEPATH%). You can define a shell environment variable KAGGLE_CONFIG_DIR to change this location to $KAGGLE_CONFIG_DIR/kaggle.json (on Windows it will be %KAGGLE_CONFIG_DIR%\kaggle.json).
  
  
  #Commands
The command line tool supports the following commands:

kaggle competitions {list, files, download, submit, submissions, leaderboard}
kaggle datasets {list, files, download, create, version, init}
kaggle kernels {list, init, push, pull, output, status}
kaggle config {view, set, unset}
  
  
  #Datasets
The API supports the following commands for Kaggle Datasets.

usage: kaggle datasets [-h]
                       {list,files,download,create,version,init,metadata,status} ...

optional arguments:
  -h, --help            show this help message and exit

#commands:
  {list,files,download,create,version,init,metadata, status}
    list                List available datasets
    files               List dataset files
    download            Download dataset files
    create              Create a new dataset
    version             Create a new dataset version
    init                Initialize metadata file for dataset creation
    metadata            Download metadata about a dataset
    status              Get the creation status for a dataset
  
 #License
The Kaggle API is released under the Apache 2.0 license.
