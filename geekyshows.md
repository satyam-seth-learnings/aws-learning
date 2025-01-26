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
