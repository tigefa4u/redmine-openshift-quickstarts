redmine-openshift-quickstarts
=============================

Redmine 2.3.4 is a flexible project management web application. Written using the Ruby on Rails framework, it is cross-platform and cross-database.

### Install Instants

```sh
rhc app create <app-name> ruby-1.9 mysql-5.1 --from-code https://github.com/tigefa4u/redmine-openshift-quickstarts.git
```

### Install push

```sh
$ rhc app create <app-name> ruby-1.9 mysql-5.1
$ cd <app-name>
$ git remote add upstream -m master https://github.com/tigefa4u/redmine-openshift-quickstarts.git
$ git pull -s recursive -X theirs upstream master
$ git push
```

### Change redmine version

change this line 16 [.openshift](https://github.com/tigefa4u/redmine-openshift-quickstarts/blob/master/.openshift/action_hooks/build#L16) [view latest version](http://www.redmine.org/projects/redmine/wiki/Download)

```sh
wget http://www.redmine.org/releases/redmine-2.3.4.tar.gz
```

