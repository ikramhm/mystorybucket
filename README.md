# mystorybucket

MyStoryBucket was my very first project using AWS. I built this system in March 2022, ahead of some internship applications, in the hope of demonstrating the skills I had gained from my newly acquired AWS Certified Cloud Practioner Certificate.

The Architecture of the bucket is as follows:

![image](https://user-images.githubusercontent.com/98710900/202315940-df6d53af-ecd5-44f6-ae55-9cbfcff21325.png)

The system uses Route53 for DNS management and leverages AWS CloudFront to deliver my content throughout the world. By utilising CloudFront and Certifcate Manager, I leveraged an SSL certificate to secure netork community to the website. This also allowed me to keep my S3 bucket private through Origin Access Identity provisions. From the developer's perspective, I created a pipeline from GitHub to the S3 bucket, using CodePipeline. The most difficult implemention (something which I added many months later) was a Lambda Function which invalidated the CloudFront cache when a new commit was made!

Luckily, I had the chance to work as a Cloud Consultant for a start-up charity where I replicated this system for a test-deployment. During this process, I created thorough documentation with detailed instructions on implementation, and conducted a presentation for the trustees on why this solution is ideal for one of their digital products.

As if this was a medium post, I will mention a few of idiosyncracies of this project.

1. Coding&Motivations

Now, I learnt HTML and CSS in Year 10, as a school project for ICT. We created a travel website with hyper-links, images and text. The code is not too disimillar to those endeavours. It is simple HTML code, which utilises CSS for a sleek and proffesional look.

The aim of this website was to describe "My Story", How I gave-up two highly saught-after vacation schemes at Silver cirle Law firms in search for a career in the clouds.

2. The website is no longer live (unfortunate story there). This is what the website looked like when it was live. 

![mystorybucketIHM](https://user-images.githubusercontent.com/98710900/212924384-b42fd2c9-60b0-47d2-be31-31f0c3daa1d0.jpg)

If, for some reason, you want to read my content, you can look at my source code!


3. In my effort to update this, I have been working on a terraform project to manually deploy the infrastructure required for this implementation. Some of the working code can be found in my terraform repo.



