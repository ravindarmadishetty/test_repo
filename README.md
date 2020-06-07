# get the sources
git clone https://github.com/ravindarmadishetty/test_repo.git

cd heroku-docker-r-shiny-app

# optionally, reinitialize git
rm -rf .git
git init
git add --all
git commit -m "initial"

# create a new heroku application and deploye
heroku create --stack=container
git push heroku master

# view the application
heroku open
