cd "Documents\Python Scripts\Tuto\Dash\dashBuildDashboardSt\DashApp"

# Requirements files

Permet de lister les lib necessaires \
lancer dans l'env de l'application \
(Buster) C:\Users\Utilisateur\Documents\Python Scripts\
Tuto\Dash\dashBuildDashboardSt\DashApp>pip freeze > requirements.txt

  pip freeze > requirements.txt

# Ajouter .ebignore


# nstall the EB CLI using pip.
NE MARCHE PAS
PASSER par codePipeline
dans l'env Buster
git clone https://github.com/aws/aws-elastic-beanstalk-cli-setup.git

In PowerShell and from the Command Prompt window:
python .\aws-elastic-beanstalk-cli-setup\scripts\ebcli_installer.py

If you encounter an error with the message "No module named 'virtualenv'", use the following commands to install virtualenv and the EB CLI:
pip uninstall -y virtualenv
pip install virtualenv
python .\aws-elastic-beanstalk-cli-setup\scripts\ebcli_installer.py

To complete installation, ensure `eb` is in PATH. You can ensure this by executing:
    1. CMD Prompt:
        cmd.exe /c "C:\Users\Utilisateur\.ebcli-virtual-env\executables\path_exporter.bat"
    2. PowerShell:
        & "C:\Users\Utilisateur\.ebcli-virtual-env\executables\path_exporter.vbs"


NOTE: Additionally, you would need to **restart this shell**

donc:
& "C:\Users\Utilisateur\.ebcli-virtual-env\executables\path_exporter.vbs"

Path in W7:
C:\Users\Utilisateur\AppData\Local\Programs\Python\Python37-32\Scripts\;
C:\Users\Utilisateur\AppData\Local\Programs\Python\Python37-32\;
C:\Users\Utilisateur\.ebcli-virtual-env\executables

where eb
eb --version

# Pour créer un environnement et déployer votre application Flask
par codePipeline
https://www.youtube.com/watch?v=4tDjVFbi31o

utilise github
## A new repo from an existing project
demmarrer gitBash dans repertoire /dashBuildDashboardSt/DashApp
git init
git add .
git status
git commit -m "text des modications"
# ajout repose

##git remote add origin https://github.com/dhazel38/essai1.git
$ git remote -v
origin  https://github.com/dhazel38/essai1.git (fetch)
origin  https://github.com/dhazel38/essai1.git (push)
...
git remote remove origin
git remote add origin https://github.com/dhazel38/flaskEssai.git
git remote -v
git push -u origin master #  and '-u' flag is upstream, which is equivalent to '-set-upstream.' 

