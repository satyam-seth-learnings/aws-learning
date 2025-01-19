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

- Install packages in Amazon Linux

  ```sh
  dnf install <package-name>
  ```

- Default user for Amazon Linux is `ec2-user`
