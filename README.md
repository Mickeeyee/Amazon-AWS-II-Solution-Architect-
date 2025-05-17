🖥️ AWS Solutions Architect 

# ☕ Static Website for the Café

This project is part of a multi-phase challenge lab focused on building a modern, cloud-based infrastructure for a fictional café. In this first challenge, I was tasked with building and hosting a static website using **Amazon S3**.

---

## 🎯 Objective

Create and launch a static website that visually represents the café and provides essential business information such as location, operating hours, and contact details.


## 🚀 What I Did

### ✅ Step 1: Created an Amazon S3 Bucket for hosting static website
- Named the bucket based on the café's domain (e.g., `my-cafe-website`).
- Creating a S3 bucket first ![image](https://github.com/user-attachments/assets/3e4033e4-34cc-4872-b409-2b68d1bb3b2c)
- ![image](https://github.com/user-attachments/assets/33ba3ad5-572f-4602-a001-d46bf7289833) 
- uploading files to the S3 bucket ![image](https://github.com/user-attachments/assets/044a28d3-87a2-4f84-bc8f-e98c61311266)
- ![image](https://github.com/user-attachments/assets/d5410efe-8279-49f1-bf1a-79004f3564de) ![image](https://github.com/user-attachments/assets/9b7a379f-b787-49ef-a285-f5defc5df13b)
- ![image](https://github.com/user-attachments/assets/ea099d55-bad6-48a8-8127-4d2a2b4f237d)
- Static web hosting ![image](https://github.com/user-attachments/assets/5c42c4f9-fa7a-4ee9-9b98-90e37f266831) ![image](https://github.com/user-attachments/assets/e44d3531-dcc4-479a-946c-c91eaa04c035)
- Creating a bucket policy to grant public read access ![image](https://github.com/user-attachments/assets/700e8793-a967-4f01-809b-15038c24ef54)
-  Website connects ![image](https://github.com/user-attachments/assets/3cdec618-55fd-4702-9e76-df4140f50d64)

### ✅ Step 2: Dynamic Website for the Cafe
-EC2 instance ![image](https://github.com/user-attachments/assets/e92f79df-10ba-40be-ba2c-3f633cdb6c1d)
-start the web server, install the database, and set them to start automatically after any future EC2 instance restarts
![image](https://github.com/user-attachments/assets/ab5c89f0-44a7-4009-83c6-f2b230959a4d) ![image](https://github.com/user-attachments/assets/9a3a57c1-4d3b-43e9-867f-de46391ff4c5)
verify database ![image](https://github.com/user-attachments/assets/bdb1d87a-6d2e-4b78-a199-316a16141fe6) ![image](https://github.com/user-attachments/assets/d3b1511a-6755-42b1-b37f-96947321a304)
MariaDB ![image](https://github.com/user-attachments/assets/dcec0c0e-11f7-4d8d-8460-dda786445b66) ![image](https://github.com/user-attachments/assets/ac8f6832-1394-42cc-947f-7ccbd8fbe41f)
Not secure just the first output / we can secure it with HTTPS ![image](https://github.com/user-attachments/assets/5b86b166-ab74-4ea8-bc22-9159fcb0092e) 

-Installing a dynamic website application on the EC2 instance 
Unzip setup.zip and db.zip file ![image](https://github.com/user-attachments/assets/b58cb648-b728-4b93-8d18-065779d3eb6a) ![image](https://github.com/user-attachments/assets/b1575548-d286-4066-8aff-4d70d76e3859)
Cafe.zip ![image](https://github.com/user-attachments/assets/bae863a7-858d-42ca-a462-84a05f189047) ![image](https://github.com/user-attachments/assets/b287b073-960a-412e-874d-ef387ce076ce)
Set app parameters ![image](https://github.com/user-attachments/assets/e2d4accf-259c-4d37-a7c8-84add3fbc8ba) ![image](https://github.com/user-attachments/assets/a40af746-4cb5-4dc0-b9a7-0a226a0509a3)
Configuring the MySQL database to support the café application, in the AWS Cloud9 bash terminal:
![image](https://github.com/user-attachments/assets/8bb43d71-59d5-40e1-8ef2-3f3255853cad) ![image](https://github.com/user-attachments/assets/abb875d6-5d9f-48ef-9016-70e3995a9654)
![image](https://github.com/user-attachments/assets/45af5b2e-5769-4622-a87f-9fbe17b0e501) ![image](https://github.com/user-attachments/assets/abcc9fd2-2119-4fd4-a4df-ed6e83817426)
![image](https://github.com/user-attachments/assets/a90cce9d-bd08-41a7-8223-3d4aaf8410e1) ![image](https://github.com/user-attachments/assets/b5001086-80b2-4e30-b0ef-8b35ac7710fb)
Testing the web application> Order submitted > Order History
![image](https://github.com/user-attachments/assets/23ada38e-442c-4584-9b3b-81a5dc2f36a4) ![image](https://github.com/user-attachments/assets/f3528773-9871-4a8e-b856-871ea1bb4553)


### ✅ Step 3: Creating an AMI and launching another EC2 instance for second region
-static internal hostname and create a new key pair on the EC2 instance ![image](https://github.com/user-attachments/assets/96163c27-aad7-4880-8249-99413e4cdcfb)
Attached role ![image](https://github.com/user-attachments/assets/3e409968-483e-417a-a960-c89461568f99) 
Creating AMI (Image) : ![image](https://github.com/user-attachments/assets/ed2760ca-66a1-4799-baf8-1ccd24ec6eeb) ![image](https://github.com/user-attachments/assets/5b883ff1-40f4-4041-9277-44544e1a9f2a)
Amazon Machine Images available ![image](https://github.com/user-attachments/assets/4f4bb5d5-9239-4d36-9130-b23a37bba611)
Copying AMI to another region(Oregon) ![image](https://github.com/user-attachments/assets/ebfe8013-a0e8-41d7-9c0e-19e6d92e035a) 
Creating new café instance ![image](https://github.com/user-attachments/assets/29149bba-65c1-4a36-a724-95c6c6609d24) ![image](https://github.com/user-attachments/assets/413d0619-5446-4d86-ae21-438f27d2b6b2)
![image](https://github.com/user-attachments/assets/c30047b5-a41d-4e4c-9d99-07bbb9a2dad8) role we created ![image](https://github.com/user-attachments/assets/b8ad0d37-abb8-4142-8561-ecc35e8f7663)
New EC2  ![image](https://github.com/user-attachments/assets/2460235c-2011-47ca-98d1-f174372fbe70) 

### ✅ Step 4: Creating a Bastion host Networking Environment for the Café
-Creating a public subnet ![image](https://github.com/user-attachments/assets/eb7d6376-65f0-4e17-8475-53d3968cf16e) ![image](https://github.com/user-attachments/assets/935b2a79-3d33-4f86-a255-fdf13bbde949)
-Attaching internet gateway to the VPC ![image](https://github.com/user-attachments/assets/d46b64d5-891f-43df-bb3b-1eb9efdcd7fa) ![image](https://github.com/user-attachments/assets/d110b79e-2d10-4225-ac1a-ea2291547388) 
 Creating a bastion host ![image](https://github.com/user-attachments/assets/36db379b-09ee-464c-a403-610924e119b1) ![image](https://github.com/user-attachments/assets/1a09e5bf-cd28-49d6-9f57-8b95e6170f3d)
 ![image](https://github.com/user-attachments/assets/98ad959e-97b1-443c-b6c8-182d3c1354eb) ![image](https://github.com/user-attachments/assets/0501522f-aa0d-4128-9fd8-90cbe5e37b02)
 Testing the connection to the bastion host ![image](https://github.com/user-attachments/assets/da4a265e-ca30-428f-b483-a3af503469e6) 
 Creating a private subnet ![image](https://github.com/user-attachments/assets/c732b8cd-0757-49b9-9b08-4210208aea80) 
 Creating a NAT gateway ![image](https://github.com/user-attachments/assets/beee736f-e27d-4a19-8bbc-bbe2891b2743) ![image](https://github.com/user-attachments/assets/9293e5f2-3bcb-4bda-8ad0-d270d6a1e301)
 Creating an EC2 instance in the private subnet  ![image](https://github.com/user-attachments/assets/b7c6b433-465d-4edb-a3d7-2a6f40931095)
 vockey key ![image](https://github.com/user-attachments/assets/a579f32f-6b16-4176-8de0-18af95d50e01) 
 EC2 ![image](https://github.com/user-attachments/assets/b0e18fb8-ce70-4afc-92f6-d71b5c275e24) ![image](https://github.com/user-attachments/assets/8a167db4-5b79-47b6-8421-d9ad0db713ee)
 ![image](https://github.com/user-attachments/assets/c9832d82-355e-4a32-a2b5-2ba244bef23a) 






 


 












## 📈 Outcome

The café's static website is now publicly accessible and provides a polished, professional digital presence. This initial deployment lays the groundwork for further phases, including dynamic features, serverless enhancements, and scalability improvements.

---

## 🛠️ Key AWS Services Used

- **Amazon S3** – For hosting the static website.
- **Amazon Route 53 (optional)** – For custom domain name mapping (if required).
- **AWS IAM** – To manage access permissions securely.

