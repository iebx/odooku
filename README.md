
# Odooku
Run Odoo on Heroku, docs at [https://adaptivdesign.github.io/odooku/](https://adaptivdesign.github.io/odooku/).

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/iebx/odooku/tree/10.0)

```
$ heroku create --buildpack https://github.com/adaptivdesign/odooku-buildpack.git#10.0
$ heroku addons:create heroku-postgresql:hobby-dev
$ heroku addons:create heroku-redis:hobby-dev
$ heroku config:set AWS_ACCESS_KEY_ID=<your_aws_key>
$ heroku config:set AWS_SECRET_ACCESS_KEY=<your_aws_secret>
$ heroku config:set AWS_REGION=<your_aws_region>
$ heroku config:set S3_BUCKET=<your_s3_bucket_name>
$ git push heroku master
```
