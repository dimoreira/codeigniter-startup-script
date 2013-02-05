# CodeIgniter Startup Script

This Bash script automates the setup of a CodeIgniter project.
It downloads the [ECodeigniter template](https://github.com/Estilingue/ECodeigniter), setups some Git and Apache files and does the *Initial Commit* for repository.
Read more about the executed operations in the **Processes** section below.

## Requirements

1. cURL
2. Git

## Processes

1. Create the specified directory based on the project name provided
2. Get the latest version of ECodeigniter (Codeigniter Template)
3. Extract Zip
4. Remove all index.html files and replace main .htaccess file with file provided in templates
5. Chmod cache and log folders to 755
6. Move basic .gitignore into place and create initial Git commit
7. Provide text instructions to complete setup

## Configuration

1. Review the files within the 'templates' folder. We've set them up how we like them, but that may not be best for you.
2. Make sure that the Bash script is in your environment PATH

## Usage

	// create a CI project in the new_project folder with default settings
	$ setupci new_project

	// create a CI project in the new_project folder without Git
	$ setupci new_project --no-git

## To Do's

1. Better handling of command line options. Right now they have to be in the specified order.
2. Add a --quiet option to limit output
