# amazon-rekognition
This repository aims to show how to use Amazon Rekognition API in Jupyter Notebook.

### Virtual Kernel

<i>Python applications will often use packages and modules that don’t come as part of the standard library. Applications will sometimes need a specific version of a library, because the application may require that a particular bug has been fixed or the application may be written using an obsolete version of the library’s interface.</i>

##### Therefore we will be using our customized kernel insted of standard Python3. You just need to run several commands given below:

* **Firstly, install jupyter**
    * pip install -U jupyter
    
* **Then create your virtual environment**
    * virtualenv ipyenv 
        * Note that you should have virtualenv installed. 
            * [sudo] pip install virtualenv

* **Activate your virtual environment**
    * source ipyenv/bin/activate

* **Install ipykernel in your virtual environment**
    * pip install ipykernel

* **Lastly, add python and ipykernel specific in the virtual environment to jupyter notebook**
    * python -m ipykernel install --user --name=ipyenv

* **Installing required modules**
	* You can simply run ***pip install -r requirements.txt***

* Now, when you run **<i>jupyter notebook</i>** command, you should see **<i>ipyenv</i>** kernel available

### AWS Command Line Interface

<i>Rekognition requires us to have our videos uploaded to S3 bucket. Therefore, you can run the following command by using [awscli](https://aws.amazon.com/cli/) to upload your videos recursively: **aws s3 cp . s3://bucket_name/ --recursive --exclude "\*" --include "\*.mp4"**</i>