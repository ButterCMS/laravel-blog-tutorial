# Butter Blog Tutorial

Code for Laravel + ButterCMS blog tutorial.

## Important Notice
This project was created as an example use case of ButterCMS in conjunction with a blog article, [How to Build a Blog with Laravel (& Send Slack Notifications)](https://buttercms.com/blog/laravel-blog-tutorial/), and will not be actively maintained. 

If you’re interested in exploring the best, most up-to-date way to integrate Butter into PhP frameworks like Laravel, you can check out the following resources:

### Starter Projects

The following turn-key starters are fully integrated with dynamic sample content from your ButterCMS account, including main menu, pages, blog posts, categories, and tags, all with a beautiful, custom theme with already-implemented search functionality. All of the included sample content is automatically created in your account dashboard when you sign up for a free trial of ButterCMS.
- [Laravel Starter](https://buttercms.com/starters/laravel-starter-project/)
- [Angular Starter](https://buttercms.com/starters/angular-starter-project/)
- [React Starter](https://buttercms.com/starters/react-starter-project/)
- [Vue.js Starter](https://buttercms.com/starters/vuejs-starter-project/)
- Or see a list of all our [currently-maintained starters](https://buttercms.com/starters/). (Over a dozen and counting!)

### Other Resources
- Check out the [official ButterCMS Docs](https://buttercms.com/docs/)
- Check out the [official ButterCMS API docs](https://buttercms.com/docs/api/)


## Installation

After cloning this repository, run the following command to install dependencies:

```bash
composer install
```

## Configurations

Rename `.env.example` to `.env`:

```bash
mv .env.example .env
```

Then, add your ButterCMS API token and Slack Webhook URL:

```bash
BUTTER_API_KEY=
SLACK_WEBHOOK=
```

You also need to add an absolute path to your SQLite database:

```bash
DB_DATABASE=/path/to/butter-blog/database/database.sqlite
```

You can easily create an SQLite database with the following command:

```bash
touch database/database.sqlite
```

You then need to migrate the database tables:

```bash
php artisan migrate
```

And seed to add a fake user:

```bash
php artisan db:seed
```

## Run Server

Finally, you can run the server with the following command:

```bash
php artisan serve
```

This will by default run the server at `localhost:8000`.
