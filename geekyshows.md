- [YouTube Playlist Link](https://www.youtube.com/playlist?list=PLbGui_ZYuhiiP7MwyVbZn4gkkJA4r5Hqp)

- Set file permission in windows

  - Syntax:-
    
    ```sh
    icacls <path_to_file_or_folder> /grant <username>:(<permissions>)
    ```

  - Example:-
  
    ```sh
    icacls "C:\example\file.txt" /grant User:R
    ```

- SSH to EC2 instance

  - Syntax:-

    ```sh
    ssh -i <shh-key-file-path> <user-name>@<instance-public-ip>
    ```

  - Example:-
 
    ```sh
    ssh -i awskey.pem ec2-user@3.7.248.65
    ```

- Default user for Amazon Linux is `ec2-user`

- Install packages in Amazon Linux

  ```sh
  dnf install <package-name>
  ```

- [Install Apache MySQL and PHP in AWS EC2](https://docs.aws.amazon.com/linux/al2023/ug/ec2-lamp-amazon-linux-2023.html)

- [Run commands when you launch an EC2 instance with user data input
](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/user-data.html)

- [Amazon Machine Images in Amazon EC2](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIs.html)

- [Placement groups for your Amazon EC2 instances](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/placement-groups.html)

- AWS Load Balancer What is Load Balancer Type of Load Balancer instance user data

  ```sh
  #!/bin/bash
  
  # Update the package list and install Apache
  dnf update -y
  dnf install -y httpd
  
  # Start the Apache service and enable it to start on boot
  systemctl start httpd
  systemctl enable httpd
  
  # Create a simple web page
  echo "Hello Instance 1" > /var/www/html/index.html
  
  # Restart Apache to apply changes (optional)
  systemctl restart httpd
  ```

- [Auto Scaling groups](https://docs.aws.amazon.com/autoscaling/ec2/userguide/auto-scaling-groups.html)

- [AWS Elastic Block Store EBS](https://youtu.be/nhds4IbMUIk?si=t3sik1LWAu1vJAQl)

  - List information about block devices, such as hard drives, SSDs, and their partitions
  
    ```sh
    lsblk
    ```
  
  - Format a partition or disk
  
    ```
    sudo mkfs.ext4 <disk/partition>
    ```

  - Mount a disk

    ```sh
    sudo mount <disk> <mount-dir>
    ```

  - Auto mount disk on system reboot
  
    - Open fstab using nano

      ```sh
      sudo nano /etc/fstab
      ```
    
    - Write content

      ```config
      /dev/xdbd       /data   ext4    defaults,nofail 0       2
      ```

- [Amazon Elastic File System](https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html)

  - [Manually installing the Amazon EFS client](https://docs.aws.amazon.com/efs/latest/ug/installing-amazon-efs-utils.html) 

- [AWS S3](https://docs.aws.amazon.com/s3/)

  - [Amazon S3 Pricing](https://aws.amazon.com/s3/pricing/)

  - [Bucket Policy Examples](https://docs.aws.amazon.com/AmazonS3/latest/userguide/example-bucket-policies.html?icmpid=docs_amazons3_console)

- [Configuring a webpage redirect](https://docs.aws.amazon.com/AmazonS3/latest/userguide/how-to-page-redirect.html)

