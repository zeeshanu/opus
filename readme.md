<p align="center">
<a href="http://i.imgur.com/Oxh9Mhg.png"><img src="http://i.imgur.com/AfFX7vQ.png"/></a>
</p>

#

<p align="center">
Opensource knowledge base application for Teams.
</p>

<p align="center">
  <a href="https://travis-ci.org/ziishaned/opus">
    <img src="https://img.shields.io/travis/ziishaned/opus/master.svg?style=flat-square"/>
  </a>
  <a href="https://opencollective.com/opus" alt="Financial Contributors on Open Collective"><img src="https://opencollective.com/opus/all/badge.svg?label=financial+contributors" />
  </a>
  <a href="https://twitter.com/ziishaned">
    <img src="https://img.shields.io/twitter/follow/ziishaned.svg?style=social" />
  </a>
  <a href="https://github.com/ziishaned">
    <img src="https://img.shields.io/github/followers/ziishaned.svg?label=Follow%20%40ziishaned&style=social" />
  </a>
</p>

## Introduction

Opus is a place for your team to document who you are, what you do and how you do it. It helps you create and maintain a knowledge base for your teams.

![Opus](http://i.imgur.com/WZvXEXY.png)

## Motivation
As companies grow, it becomes difficult to manage and communicate the knowledge across different departments, Opus acts as a single source of truth; a go-to place for the employees to get knowledge. It gives enterprises the power to create anything and everything; from meeting notes, project plans, product requirements, technical documentations, orchestrate processes, work-flows and more. 

There are spaces for every team, department or major project. Then employees can create, organize and share knowledge inside their relevant teams and keep work organized. There is a structured hierarchy and powerful search engine to find what you need quickly and easily. Apart from that, templates help creating documents without any hassle and there is PDF and Office Docs generation for the ease of sharing.

## Features

* Create manage Wikis (group of knowledge pages)
* Create nested pages inside wikis
* Manage wikis and pages by spaces and tags
* Invite employees by email
* Powerful ACL to assign different roles and permissions to employees.
* Slack notifications for the wiki updates
* Mark wikis and pages as favorite
* Watch wiki/pages to get notified
* In-app notifications
* Discussions using comments
* Create reusable page templates
* Search across the knowledge base
* ..and more

## Screenshots

You can find some screenshots of the application in this following [link](https://github.com/ziishaned/opus/blob/master/demo.md).

## Installation

You can use one of the following methods:

* [Docker](#docker)
* [Localhost](#localhost)

### Docker

```bash
composer create-project ziishaned/opus
cd opus
cp .env.dist .env
docker-compose up
docker-compose exec app php artisan key:generate
docker-compose exec app php artisan migrate
docker run -v "$PWD":/var/www/ opus_app /usr/local/bin/composer install
```

### Localhost

- Run the below command in your terminal:
  ```bash
  composer create-project ziishaned/opus
  ```
- Create `.env` using `.env.dist` and populate the relevant information
- Install the dependencies
  ```bash
  composer install
  ```
- Open the project directory and run the below
  ```bash
  php artisan migrate
  ``` 
- Generate an application key
  ```bash
  php artisan key:generate
  ```
- Run the database seeder
  ```bash
  php artisan db:seed
  ```

## Contributions

* Report issues
* Spread the word
* Reach out to me directly at ziishaned@gmail.com or on twitter [@ziishaned](https://twitter.com/ziishaned)

## Contributors

### Code Contributors

This project exists thanks to all the people who contribute. [[Contribute](CONTRIBUTING.md)].
<a href="https://github.com/ziishaned/opus/graphs/contributors"><img src="https://opencollective.com/opus/contributors.svg?width=890&button=false" /></a>

### Financial Contributors

Become a financial contributor and help us sustain our community. [[Contribute](https://opencollective.com/opus/contribute)]

#### Individuals

<a href="https://opencollective.com/opus"><img src="https://opencollective.com/opus/individuals.svg?width=890"></a>

#### Organizations

Support this project with your organization. Your logo will show up here with a link to your website. [[Contribute](https://opencollective.com/opus/contribute)]

<a href="https://opencollective.com/opus/organization/0/website"><img src="https://opencollective.com/opus/organization/0/avatar.svg"></a>
<a href="https://opencollective.com/opus/organization/1/website"><img src="https://opencollective.com/opus/organization/1/avatar.svg"></a>
<a href="https://opencollective.com/opus/organization/2/website"><img src="https://opencollective.com/opus/organization/2/avatar.svg"></a>
<a href="https://opencollective.com/opus/organization/3/website"><img src="https://opencollective.com/opus/organization/3/avatar.svg"></a>
<a href="https://opencollective.com/opus/organization/4/website"><img src="https://opencollective.com/opus/organization/4/avatar.svg"></a>
<a href="https://opencollective.com/opus/organization/5/website"><img src="https://opencollective.com/opus/organization/5/avatar.svg"></a>
<a href="https://opencollective.com/opus/organization/6/website"><img src="https://opencollective.com/opus/organization/6/avatar.svg"></a>
<a href="https://opencollective.com/opus/organization/7/website"><img src="https://opencollective.com/opus/organization/7/avatar.svg"></a>
<a href="https://opencollective.com/opus/organization/8/website"><img src="https://opencollective.com/opus/organization/8/avatar.svg"></a>
<a href="https://opencollective.com/opus/organization/9/website"><img src="https://opencollective.com/opus/organization/9/avatar.svg"></a>

## License

The license holder is allowed to use the software for free, as long as they don't make money using it. [Read more in License](https://github.com/ziishaned/opus/blob/master/LICENSE.md)
