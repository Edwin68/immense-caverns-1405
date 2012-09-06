web: bundle exec thin -R config.ru start -p $PORT -e ${RACK_ENV:-development}
worker: bundle exec rake resque:work QUEUE=*
clock:  bundle exec rake resque:scheduler