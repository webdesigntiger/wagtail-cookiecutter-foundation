Installation
============

Let's pretend you want to create a Django project called "wagtail_project". Rather than using `startproject` and then editing the results to include your name, email, and various configuration issues that always get forgotten until the worst possible moment, get cookiecutter_ to do all the work.

.. _cookiecutter: https://github.com/audreyr/cookiecutter

First, get Cookiecutter ::

    $ pip install cookiecutter

Now run it against this repo::

    $ cookiecutter https://github.com/chrisdev/wagtail-cookiecutter-foundation.git

You'll be prompted for some values. Provide them, then a Django project will be created for you ::

    Cloning into 'wagtail-cookiecutter-foundation'...
    remote: Counting objects: 5085, done.
    remote: Compressing objects: 100% (172/172), done.
    remote: Total 5085 (delta 21), reused 0 (delta 0), pack-reused 4911
    Receiving objects: 100% (5085/5085), 11.74 MiB | 2.07 MiB/s, done.
    Resolving deltas: 100% (2818/2818), done.
    Checking connectivity... done.
    project_name [Wagtail Project]: 
    repo_name [wagtail_project]: 
    version_control_system [git]: 
    vcs_repo_username [bitbucket_username]: 
    vcs_repo_hostname [bitbucket.org]: 
    author_name [Your Name]: 
    email [Your email]: 
    description [A short description of the project.]: 
    timezone [UTC]: 
    now [2015/04/16]: 
    year [2015]: 
    production_host_name [wagtail-example.org]: 
    use_ssl_in_production [true]: 
    staging_host_name [staging.example.org]: 
    use_vagrant_staging [True]: 
    deploy_user_name [django]: 
    django_admin_user [my_wagtail_admin]:

Enter the project and take a look around::

    $ cd wagtail_project/
    $ ls

Create a git repo and push it there::

    $ git init
    $ git add .
    $ git commit -m "first awesome commit"
    $ git remote add origin git@github.com:cclarke/my_site.git
    $ git push -u origin master