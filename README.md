# docker-compose run Drupal 8 with drupal-composer/drupal-project

## build it!
	docker build -t="guoxiangke/drupal-composer" . --no-cache
	docker push guoxiangke/drupal-composer
## start it
	docker-compose -p drupal8 up -d  --build --remove-orphans --force-recreate
## stop it
	docker-compose -p drupal8 down