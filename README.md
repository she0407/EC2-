# **EC2 Basics**

---

## **EC2 Instance Launch Using Windows AMI**

1. Navigate to the AWS console and search for the EC2 service. The homepage should look like this:  
   ![EC2 Homepage](https://github.com/user-attachments/assets/a620307b-59d4-4bb5-9374-c2c376707fa6)

2. Click on **Launch Instance**, provide the name of the instance, and select the operating system (OS) you want. Here, **Windows** was chosen:  
   ![Windows AMI Selection](https://github.com/user-attachments/assets/20258dea-8c92-46c2-8250-223fca0969fb)

3. Choose the instance type and select the key pair:  
   ![Instance Type and Key Pair](https://github.com/user-attachments/assets/cbb896ce-4173-4c24-ba60-0ab43b68d6f1)

4. Configure the security group and enable **RDP traffic**:  
   ![RDP Traffic Configuration](https://github.com/user-attachments/assets/613a0854-2c7a-4106-8695-5eaf96d2bab9)

5. Launch the instance and double-check the **inbound rules** for RDP in the security group:  
   ![Security Group Inbound Rule](https://github.com/user-attachments/assets/493cd70a-7d9d-426d-bc6d-56b76fbd2a09)

6. Connect to the EC2 instance using **RDP Client**:
   - Generate the password:  
     ![Generate Password](https://github.com/user-attachments/assets/edf37582-8ea9-4ff7-bb48-ffd788624bd1)
     ![Choose Key Pair](https://github.com/user-attachments/assets/61f1ba40-67ce-4864-b062-6d911f36d889)
   - The generated password appears as follows:  
     ![Generated Password](https://github.com/user-attachments/assets/7e4a4256-2166-4aee-92b2-600cdebed09f)

7. Use **Remote Desktop Connection** to paste the **Public DNS Address** and connect:  
   ![Remote Desktop Connection](https://github.com/user-attachments/assets/9b1fe7ed-a2e6-4335-bc3e-df4ae559e028)  
   ![RDP Instance Connection](https://github.com/user-attachments/assets/35cd9897-d242-4184-adb9-fca23308e209)

---

## **EC2 Instance Launch Using Ubuntu AMI**

1. Follow the same steps as above but choose **Ubuntu AMI**.
2. Copy the **SSH command** from the instance and paste it in Git Bash:  
   ![Ubuntu AMI Selection](https://github.com/user-attachments/assets/0b34aeb9-fb62-4683-9ba8-2381d1f9dc1e)

3. Launch the instance and configure the **SSH connection**:  
   ![SSH Connection](https://github.com/user-attachments/assets/6bcc3e24-67d6-4aa7-8fa0-b0a1414180b1)

---

## **EC2 Instance Launch Using Linux AMI**

1. Select **Linux AMI**, configure the instance, and connect using Git Bash:  
   ![Linux AMI Selection](https://github.com/user-attachments/assets/4812e130-0513-4c37-a6d6-fbbbe621d4f6)  
   ![SSH Client](https://github.com/user-attachments/assets/1a5adbf7-8608-4fa3-97ed-2f365236a4fd)

2. Successfully connect to the EC2 instance via SSH:  
   ![Linux SSH Connection](https://github.com/user-attachments/assets/b534752b-808b-4fff-9477-a13289c2f6a5)

---

## **Launching an Instance Using PuTTY**

1. Convert the **.pem key pair** to **.ppk format** using PuTTYgen:  
   ![PuTTYgen Key Conversion](https://github.com/user-attachments/assets/c503b4e1-f033-42c4-831e-ca396a33d65c)

2. Open PuTTY, paste the **Public IP Address**, upload the converted key pair, and connect:  
   ![PuTTY Connection](https://github.com/user-attachments/assets/400367af-5214-4174-be06-46e8a479cc7b)

3. Successfully log in to the EC2 instance using **ec2-user**:  
   ![PuTTY EC2 Connection](https://github.com/user-attachments/assets/17202524-92e4-4187-a8b4-06d8ca82faa4)

---

## **Exploring AWS EC2 Dashboard**

- The dashboard provides various features for monitoring and managing your instance:  
  ![Dashboard](https://github.com/user-attachments/assets/5d009f83-3b0a-4718-901f-36a58eafc8e8)

### Key Features:
- **Security Tab**: View IAM roles and security group details.  
  ![Security Tab](https://github.com/user-attachments/assets/14513dfc-abfd-457f-8fcd-b684782c52c2)

- **CPU Utilization**: Monitor workload performance.  
  ![CPU Utilization](https://github.com/user-attachments/assets/e190635c-6db9-4f78-84b4-a754c525c41c)

- **Networking Tab**: Adjust and diagnose networking setups.  
  ![Networking Tab](https://github.com/user-attachments/assets/5412367c-2fc0-4bd5-87dd-34a69aeff300)

---

## **Protocols**

### Device Communication Protocols in AWS IoT Core:
- **MQTT**: Lightweight protocol for small data transfers.
- **HTTPS**: Secure website connection for one-way data transfer.
- **TLS**: Encryption layer ensuring secure communication.

### AWS API Protocols:
- **ec2**: Manage EC2 services.
- **json/rest-json**: Communication for newer AWS services.
- **query/rest-xml**: Communication for older AWS services.

### Amazon Workspaces Protocols:
- **PCoIP**: High-quality graphics streaming.
- **WSP**: Optimized for low bandwidth usage.

---

This README file is now ready to publish with enhanced readability and structure!
