
<div style="width:100%;height:0;padding-bottom:50%;position:relative;">
  <iframe src="https://giphy.com/embed/hTZJKhPJyJhv7Xry36" width="100%" height="100%" style="position:absolute" frameBorder="0" class="giphy-embed" allowFullScreen>
  </iframe>
</div>
<p>
  <a href="https://giphy.com/gifs/hTZJKhPJyJhv7Xry36">via GIPHY</a>
</p>



To use DB:

A. you can run db using Vagrant
* add 
  DBHOST = localhost
  DBUSER = development
  DBPASS = development
  DBNAME = final_project
  DBPORT = 5432
  to your .env file
* install dependancy (PG and dotenv) - run npm install

B. you can run db using PostgreSQL on your local machine:
* install postgreSQL - https://www.robinwieruch.de/postgres-sql-macos-setup
* install dependency (PG and dotenv)
* to start local db server - use command:
        pg_ctl -D /usr/local/var/postgres start
* to stop local db server - use command:
        pg_ctl -D /usr/local/var/postgres stop.


For connecting Express with Axios in both cases you need to add
"proxy": "http://localhost:5000"
to the package.json !!

For visualising data you can use Postico app. Credentials are from .env!
