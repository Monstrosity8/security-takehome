### The following questions are meant to serve as an assessment; answer as much as you are able to answer (even if you can't fully answer a specific question). Make sure to explain your answers.




1. Explain the differences between a VM, container, chroot jail, and Kubernetes pod.
2. Explain the CIA triad and provide an example of each.
3. How would you go about investigating a security incident in AWS?
4. How do you stay up to date on security news?
5. Describe the process, in as much detail as possible, that occurs when a user opens a web browser and types in <https://okcupid.com/> until the site is displayed on their browser.
6. Describe a security incident response process (either one you have been a part of or a public incident that you read about)
7. What is the principle of least privilege and why is it important? Provide an example.
8. What is a 0 day?
9. What is a CVE?
10. Explain XSS.
11. What is MFA? List the factors.

### The below is intended to test your comfort level with scripting and experience with different technologies, such as AWS, Terraform, Bash and/or Python. Please answer what you can to the best of your ability. When you complete this tasks, create .txt or a .MD called `results` with the output of the questions you completed (be sure to annotate the question number), make a directory named `submission_<your initials>` and copy all the code and the results file to the directory - Please include the answers to the questions above as well. 
### You will then encrypt the directory with our public gpg key and upload it back to our repo. (Our key is uploaded to `keys.openpgp.org` with the email `security@okcupid.com`. If you are unfamiliar with this process please use this site as reference `https://yanhan.github.io/posts/2017-09-27-how-to-use-gpg-to-encrypt-stuff/`)

1. Suppose that you have an s3 bucket, `bucket`, which contains a file, `wordlist` that contains a comma-separated list of words. Write a lambda function which will  receive a json event payload containing a query string. The Lambda function should check whether the query word is in the wordlist and place the result on an SQS queue as well as return it.

   Sample wordlist:

   ``` 
   working,for,okcupid,is,really,fun,come,join,us
   ```

   Sample request:

   ``` json
   {
     "query":"for"
   }
   ```
2. Write Terraform code to deploy the above.
3. Using the [Harry Potter API](https://hp-api.herokuapp.com/), retrieve a list of students and their houses, print a list sorted by house then alphabetical order.
4. Write a bash script to find every file owned by the user `joe` and output the number of lines in the file.
5. Create a file named `permissions.txt` and grant all permissions to the owner of the file, read permissions for the group and execute permissions for all other users. 