# ViS3Editor - Edit S3 Files Directly in Terminal

ViS3Editor is a tiny command-line tool written in JavaScript that allows you to edit file directly from Amazon S3 without leaving your terminal. It leverages the power of the Vim editor for file editing and provides a seamless workflow for handling S3 files.

> At work, we manage product configuration files on S3. Each time a configuration change is needed, it requires delving into the AWS jungle—logging in, navigating through S3, downloading the file, making edits, and then re-uploading the configuration file. This process is tedious and unnecessary, so I developed a small tool for swift edits directly without leaving my cozy command line. 

## Installation

1. **Clone the repository:**

2. **Navigate to the project directory**

3. **Install dependencies**

4. **Create a symbolic link to make the command globally accessible**

## Requirements
Vim installation on your system is recommended for better handling, but other vi editors can also be used. Along with this, node and npm is also required.

## How to Run

1. Run the command with a valid S3 path:

```
ViS3Editor s3://<bucket-name>/<path-to-file>
```

2. Follow the on-screen instructions for editing the file in Vim.

3. Save and close the editor.

4. The file will be uploaded back to the specified S3 path.

## Note
Ensure that AWS credentials are configured on your system or set up the necessary environment variables for authentication.
# TODO

- [ ] download and store locally file in tmp dir
- [ ] add --validate=json flag to extend it to do validation before uploading 
- [ ] improve the error handling 