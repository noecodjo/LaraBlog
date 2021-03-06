# Blog Using Laravel 5
### Let's keep it as simple as possible. Configure anything you want
A full-featured blogging system for personal use. Minimum library used. No frontend theme and anything heavy or unnacessary library used.  
 
### There are four several types of users with several permissions
1. Admin
  * Can manage articles and comments of other users
  * Can manage categories 
  * Can manage keywords
  * Can manage other users except Owner
2. Owner
  * Can do anything that can be done by admin

  * Create admin user

  * Change system configuration variables
3. Author
  * Can write article and can manage his own article
  * Can manage comments on his own article
4. Reader
  * Can read and comment on article providing his email address. 
  * Can subscribe to be notified for new article
  * Can search for article with
  * Can navigate article based on categories

### Technologies Used: 
1. Laravel 5.4
2. VueJS 2
3. Bootstrap 3

### Installation Process
1. Execute `git clone https://github.com/alimranahmed/Personal-Blog-Using-Laravel5.git` on your terminal to download this project.
2. Go to the project root directory and execute `composer install` to install all PHP dependencies of the project
3. Create a file named as .env and copy the content of .env.example to newly created .env file 
4. Then execute `php artisan key:generate` on your terminal/cmd to generate environment key
5. Then create a Database for this project and edit the .env file to authorized this project on your database. 
6. Execute `php artisan migrate:refresh --seed` terminal on your terminal.
7. Now you are ready to go, If you don't want to create any virtual host for this project then execute
  `php artisan server`
8. Now visit the url shown on your terminal, something like `localhost:8000`. Its running!

### Screenshot

##### Single article view
![single blog](https://cloud.githubusercontent.com/assets/7629427/23341414/5280728c-fc71-11e6-9ae4-be9405e04e40.png)

##### Admin panel view
![admin_panel](https://cloud.githubusercontent.com/assets/7629427/23618709/5e05eac4-02bb-11e7-819a-bb13d7c5b0cd.png)

### Contribution 
Anyone is always welcome to contribute on the project. If you want to work with, just create and issue(even if you want to fix the issue). After fixing any issue or adding any new feature just send a pull request, I will be happy to add your code for the betterment of this project. Thanks.

##### Note
If you cloned the project little bit earlier and after pulling the newer changes it's not working now, please execute the `composer update` command in the CLI when you are the root directory of the project. Beside, don't forge to cross match your `.env` file version with newly pulled `.env.example` file.
