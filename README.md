# Group Chat using Laravel and Pusher

This repository demonstrates the process to create a realtime *Group Chat Application* using [Laravel](https://laravel.com/) and [Pusher](https://pusher.com/). Please follow below steps to have a running version of the app in this repo

1. Clone repo
2. Configure your environment variables for Pusher and Laravel by copying the `.env.example` to `.env`
3. Add Pusher config details to bottom of the .env
4. Create a blank mysql database and change the name of the DB in the .env to match
5. Configure your Pusher key and cluster in the `resources/assets/js/bootstrap.js` file
6. Install composer dependencies
7. Run npm install
8. Run `php artisan migrate` to create database
9. Run `npm run watch`
10. In a seperate terminal window run `php artisan serve`
11. In a third terminal windoe, run `php artisan queue:listen`
12. Navigate to `localhost:8000` in two seperate browsers (or one regular and one private browser window) and register two users.
13. In one window, name a group, select the other user and create a group. You should see after a few seconds a group pop up in the other window. 
14. Write and send a message. It should be sent to the other window. 
