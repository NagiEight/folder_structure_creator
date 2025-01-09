# Folder Structure Creator

This Python script reads a text file containing a folder structure and creates the corresponding folders on your file system.

## How It Works

1. **Reading the Folder Structure**: The script reads a text file where each line represents a folder. Indentation indicates the hierarchy.
2. **Creating Folders**: It processes the file to determine the folder structure and creates the folders accordingly.
3. **Identifying the Executable's Directory**: The script identifies the directory where it is located, whether it’s frozen (compiled as an executable) or not.
4. **Locating `.txt` Files**: It searches for `.txt` files in the directory.
5. **Choosing a File**: If multiple `.txt` files are found, it prompts the user to choose one. If there’s only one, it uses that file directly.
6. **Creating Folder Structure**: The script creates the folder structure based on the text file.

## Installation

1. Ensure you have Python 3.x installed on your system. You can download it from the official [Python website](https://www.python.org/downloads/).
2. Install the `folder_structure_creator` package using pip:

```
pip install folder_structure_creator
```

3. Ensure there is a .txt file with the folder structure in the same directory as the executable.

## Usage

1. Place a text file of the folder structure in the executable's directory or `<user_home_directory>\AppData\Local\Packages\<python_distribution_directory>\LocalCache\local-packages\<python_version>\site-packages\folder_structure_creator
` if it was installed with pip.
2. Run the script.

```sh
python fstruct.py
```

3. Follow the prompts if multiple `.txt` files are found.

## Your .txt file should look like this

```plaintext
ParentFolder
 ChildFolder1
  SubChildFolder1
 ChildFolder2
```

## Requirements

- Python 3.x

## Notes

- The script can handle both spaces and tabs for indentation.
- Ensure the .txt file with the folder structure is correctly formatted.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
