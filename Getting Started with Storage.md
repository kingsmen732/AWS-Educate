# AWS Session 2 Questions and Correct Answers

1. **What is the definition of object-based storage?**  
   **Correct Answer:** Object storage is a method of storing files based on attributes and metadata.

2. **Which storage class is for raw storage of data in fixed-sized chunks, each with a unique identifier?**  
   **Correct Answer:** Block.

3. **Which option is a typical use case for Amazon S3?**  
   **Correct Answer:** Object storage for media hosting.

4. **An employee at a healthcare facility must store 7 years of patient information that is rarely accessed. Which Amazon S3 storage tier is the best choice?**  
   **Correct Answer:** Amazon S3 Glacier Deep Archive.

5. **Which of the following items are types of cloud storage available in AWS? (Select THREE.)**  
   **Correct Answers:**  
   - Object  
   - Block  
   - File  

6. **Which types of data does Amazon S3 offer encryption for? (Select TWO.)**  
   **Correct Answers:**  
   - Data in transit  
   - Data at rest  

7. **When naming an Amazon S3 bucket, a developer must choose something that is unique. For which portions of AWS must the bucket name be unique?**  
   **Correct Answer:** Globally across all AWS accounts.

8. **When a developer creates an Amazon S3 bucket, they can set access permissions. Suppose that they leave the defaults and make no changes to the settings. Who can view objects in the bucket?**  
   **Correct Answer:** Only the developer.

9. **Which storage service is recommended if a customer needs a storage layer for a database attached to an Amazon EC2 instance?**  
   **Correct Answer:** Amazon Elastic Block Store (Amazon EBS).

10. **Amazon S3 is priced based on the storage class and features that the user chooses. Which items is the user charged for? (Select THREE.)**  
    **Correct Answers:**  
    - GB storage per month  
    - PUT, copy, POST, LIST, and GET requests  
    - Transfers OUT to other Regions or the internet

11. **A developer can use Amazon S3 to configure Cross-Region Replication of objects. What is one benefit of enabling Cross-Region Replication?**  
    **Correct Answer:** Minimize latency by maintaining object copies in AWS Regions that are geographically closer to their users.

12. **A gaming company has data access patterns that are often unpredictable. Which storage class could they use to help minimize costs?**  
    **Correct Answer:** Amazon S3 Intelligent-Tiering.

13. **Lifecycle rules define the actions that Amazon S3 can apply to a group of objects to store them cost-effectively. Which two types of actions can lifecycle rules apply to an object? (Select TWO.)**  
    **Correct Answers:**  
    - Expiration actions  
    - Transition actions





# Simulation overview
- In this simulation, you use some of the Amazon Simple Storage Service (Amazon S3) features that you just learned about to create a static website.
- Static websites can contain HTML pages, images, style sheets, and all files that are needed to render a website. Static websites do not use server-side scripting or a database. However, they might contain client-side scripts that run in a user's web browser.
- You can host a static website on Amazon S3 by uploading the content and making it readable by users. No servers are needed, and you can use Amazon S3 to store and retrieve any amount of data anytime from anywhere on the web.
  
  # TASK 1 GUIDE:
  1) Click on the search --> Type `S3` --> Click on the `S3 Bucket`
  2) Click on create bucket 
  3) Bucket name --> sim-website and Enable ACLs
  4) De-select the `Block all public access` checkbox and Acknowledge the settings
  5) Enable `bucket Versioning` 
  6) Add tags 
    - key : *Department*
    - Value : *Marketing*
  7) Create `Bucket`

  # TASK 2 GUIDE:
  1) Click on `sim-website`
  2) Click on `properties tab`
  3) Scroll down and Click on Edit `Static website hosting` 
  4) Enable the `static website hosting ` option
  5) Enter `index.html` in the index document textbox
  6) Enter `error.html` in the Error document textbox 
  7) Click on `Save changes`
  8) Scroll all the way down and Click on the `Bucket website endpoint link`
  9) Error message will pop up , Click on the first tab open inside the window.

# TASK 3 GUIDE
1) Scroll all the way up and Click on `Objects`
2) Click on `Upload` button
3) Click on `Add files` button
4) Windows explorer pops up ---> Select the "Website files" and click `open`
5) Select all the files inside the `folder` and Click on `Open`
6) Scroll down and Click on `upload`button
7) Click on the `close` button

# TASK 4 GUIDE
1) Select the `403 forbidden` tab in the browser window
2) Click `Refresh button`  
3) Click back to `sim-website - S3 bucket` tab in the browser window
4) Select the `checkbox` on the left of `Name label`
5) Click on `Actions `and Choose `make public using ACL` option
6) Click on `Make public` button on the bottom
7) Click `Close` button the left top
8) Go to the `403 forbidden` tab in the browser window again
9) Click `Refresh button`  to load the website
10) Click on the "`X`" (Close button) of the website tab in the browser window.

# TASK 5 GUIDE
1) Click on `upload` button
2) Click on `add files` button
3) Windows explorer pops up ---> Select the "new-report" and click `open`
4) Scroll all the way down and click on `upload` button
5) Click the `close` button on the top right
6) Select the `checkbox` next to `new-report.png
7) Click on `Actions `and Choose `share with a presigned URL`
8) Type in `2` in the textbox for 'Number of minutes'
9) Click on the `copy presigned URL` on the Top Green Notification
10) Open a new Browser tab in the given window
11) Paste the `presigned URL` copied in previous page into the search bar and hit `Enter`
12) After the Excel sheet loads , Click on `refresh button` on the browser
13) Click on the "`X`" (Close button) of the website tab in the browser window.

# TASK 6 GUIDE
1) Click on `permissions` tab on the console
2) Scroll down to `Bucket Policy` and Click on `Edit` button
3) Go to the `blank editor space` below Policy title and Paste (content is already in your clipboard)
4) Scroll down and Click on the `save` button
5) Click on `Objects` button
6) Select the checkbox for the `index.html` file and Click on `Delete` button
7) Type `delete` in the textbox and click on `Delete objects` button
8)  Error message will come on top and Click on `close` button

# TASK 7 GUIDE
1) Open the context (right-click) menu for the `index file`
2) Choose `Open with` and Select `notepad` application
3) Click on the `highlighted part` and Type `Created by Jane` in the input field
4) Choose `File` from the Notepad menu and Select `save`
5)  Choose the `Console` running in your browser
6) Click on the `index.html` button and Choose the `Object URL` hyperlink
7) Choose the `Back` button on the browser
8) Click on `sim-website`
9) Click on `upload button` and choose `add files` button
10) Windows explorer pops up ---> Select the "Website files" and click `open`
11) Choose `index.html` file and click `open` button
12) Scroll down and click `upload` button
13) Click `close` button
14) Choose the checkbox for the `index.html` file 
15) Choose `Actions` and Choose Make `public using ACL`
16) Click on `Make public` and click on the orange `close`button
17) Choose the `index.html` file name with the hyperlink
18) Choose the `Object URL` hyperlink
19) Choose `back` and click on the `sim-website` on the top

# TASK 8 GUIDE
1) Choose the `Show versions `toggle switch
2) Choose the `scroll bar` to scroll down
