# aws-learning

[AWS Offial Website](https://aws.amazon.com)

- Set file permission in windows

  - Syntax:-
    
    ```sh
    icacls <path_to_file_or_folder> /grant <username>:(<permissions>)
    ```

  - Example:-
  
    ```sh
    icacls "C:\example\file.txt" /grant User:R
    ```
