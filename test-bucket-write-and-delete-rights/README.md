# test-bucket-write-and-delete-rights

## Description:
### Program will list all subfolders inside the given paths, will try to write into each and if writing was successful then it will try to delete the previously written file, providing output to the user and writing to output file at the end.
### Things to be taken into account:
### 1. If write was successful, but deletion wasn't, you will have to clean up the files by hand.
### 2. If file is already inside the bucket folder, and you don't have deletion rights, the write test will not work properly (You will receive a [?] warning).
### 3. If couldn't write, then deletion test will not happen.
### Requirements: gsutil, being authenticated with gsutil
### Arguments: 
### -iF (or --bucketfolderslist) pathToInputFile (containing buckets separated by new lines) [Default is "listOfOpenBuckets.txt"]
### -tF (or --testfile) pathToTestFile (file to upload) [Default is "testfile"]
## To run simply execute the script.
### Example 1: python testGCPBucketsWriteRights.py
### Example 2: python testGCPBucketsWriteRights.py -iF C:\Users\BauBau\Documents\bucketsToTest.txt -tF C:\Users\BauBau\Documents\myCustomTestFile.txt
## Output files will be generated inside the output folder once script finishes.

## Demo
![](demo.gif)