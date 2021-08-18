<p align="center"><a href="https://phpreel.org/" target="_blank"><img src="https://developer.phpreel.org/img/logo.png" width="250"></a></p>

# phpReel Static Laravel Package
[phpReel](https://phpreel.org/) Static is a simple Laravel Package created and used by [phpReel](https://github.com/phpreel/phpreel) that converts your Laravel application to a static HTML website.

You only have one artisan command `php artisan generate:static` which will generate your static website. Once you run this command you will find your static website in a directory called `static`, right at the root of your Laravel application.

You can add a .gitignore file to the `static` directory and restrict the files that can be committed. Here is the `.gitignore` file used by [phpReel](https://github.com/phpreel/phpreel).

```
*
*/
!.gitignore
```

Make sure you have your Laravel application running on a server before executing the command. You can start a server in seconds by running `php artisan serve` into your terminal. Don't close the server when you are running `php artisan generate:static`, just use two terminals if needed.

> Keep in mind that a some of the functionality that your Laravel app offered might not be available anymore on your static website (you will not have access to a database, login system, payments and so on).

## Installation
You can install the package via composer.
```
composer require phpreel/static
```

## Why to use phpReel Static?
The main benefit of having static websites is the fact that you can deploy them anywhere from GitHub Pages to Netlify or even Google Drive. This means that is very easy and cheap to have your own website on the internet.

## How to update a website generated by phpReel Static
You should run your Laravel application and make your modifications there (stuff like adding a new article, updating something and so on). Once you are done, run the command `php artisan generate:static` and deploy the newly generated static website directly to your provider.

## Contributing
phpReel is getting bigger and better each day, thus with every new feature, it becomes more and more difficult to manage a product without a team. I really want to grow this project into a full-blown software company but until that day I rely entirely on the help of the community. Here is a list of things you can do to help phpReel grow:

- [Fork the project on GitHub](https://github.com/phpreel/static/) and contribute to it by adding new features, fixing bugs, or improving on what's already there (then submit a pull request)
- Spread the word about the project
- Just simply use it and open an [issue on GitHub](https://github.com/phpreel/static/issues) if you find any bugs

## License
[MIT](https://github.com/phpreel/phpreel/blob/main/LICENSE)
