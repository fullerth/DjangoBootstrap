# Overview
Simple Project to quickly get a new Django environment up and running

## Using the Project
1. Create a new repo on github with <new-repo-name>
1. `git clone https://github.com/fullerth/DjangoSetup.git <new-repo-name>`
1. Change the new repo origin to <new-repo-url>
  ```
  git remote rm origin
  git remote add origin <new-repo-url>
  ```
1. Edit this README.md to discuss the new project.
1. Checkin and push to test the new repo
1. Create a virtual environment
  * `python3 -m venv <new-repo-name>_venv`
1. Install requirements
  * `pip install -r requirements.txt`
1. Make a Django site

## Templates
Both project and app templates for django-admin/manage.py are provided.

To create a project, from the root directory use:
`django-admin startproject --template project_template <project-name> source`

To create a new application with the template use:
`manage.py startapp --template <path-to-app-template> <app-name>`

## Virtual Environment
The project will ignore a virtual environment in django_setup_venv. After 
cloning the project change this in .gitignore to a sane value for the new 
project.
