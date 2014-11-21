# DrupalCores
![count all the git commits](https://github.com/ericduran/drupalcores/raw/pystart/img.jpg)

Ruby script to parse all the git commit, aggregate every users commit count and generate
a flat html page for easy viewing for all the contributes and commit counts.

## Instructions
First you need to clone a copy of the drupal 8 branch into your drupalcores directory

    git clone --branch 8.0.x http://git.drupal.org/project/drupal.git
    git clone --branch gh-pages git@github.com:lauriii/drupalcores.git pages

Once you have a git repo of drupal core in the drupal directory then you can run the cores.rb script

    ./cores.rb

For the company list do:

    ./companies.rb > pages/companies.html

Takes a long time for the first parsing... (~1.5h)
After that it uses the company_mapping.yml and company_infos.yml.

The companies.rb accepts a parameter to either force a update of all people and companies (--update-all)
or to update people, which were not found (--update-not-found).

View online:
 [DrupalCores.com](http://www.drupalcores.com/)

Do you only want the data?
 [BAM!!!](http://www.drupalcores.com/data.json)

##Help:

If you want to help please just fork the project and issue a pull request.
