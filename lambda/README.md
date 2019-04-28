# Lambda tools  
Here you can find simple aws lambda tools such as uploading and downloading functions. This is useful if you are using git as source control and don't want to hassle through the management console.  
  
# upload_lambda
This tool allows for quick uploads to lambda using awscli. It takes one argument which is the source folder. Use it from one directory above the source. This script zips the source up and uploads it using the cli's lambda command in conjunction with upload zip. After it's uploaded, the zip is removed.  
  
# download_lambda
Like upload_lambda, this tool uses awscli to download a specified lambda function by name. It will download the zip file, unpack it into a directory of the same name (first create it if it doesn't exist), then remove the zip.
