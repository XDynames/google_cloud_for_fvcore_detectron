# Google Cloud Storage for fvcore based libraries
cloud_utils.py can be imported as part of detectron2 to give full support to paths to remote resources host on google cloud store with prefix gs://

By installing tensorflow in the environment your project runs tensorboard will also log to the remote bucket and can be accessed locally with `tensorboard --logdir "gs://bucket-name/output-directory"` 

To run the test harness modify cloud_utils_tests.py by adding a project and bucket to the setUpClass() method you are authenticated to access. Then upload the included test2.txt file to your bucket at gs://bucket_name/test/path/text2.txt.