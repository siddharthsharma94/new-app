## New App Template

Over time i've realized I have an optimal way of deploying apps. I end up doing the same things to set up the repos / dev ops deployments of the apps I'm creating. This monorepo deployment, serves to easily deploy and scaffold my apps.

My Stack uses `Vercel + Railway`

## How to use

- Click the Use Template Button on the top of this page.
- Go to Vercel.com and link to Github, and connect to your newly created repo. Select the web folder and deploy.

  - to only build the vercel app on changes to web, go to git section and add the following to the ignore build step `git diff HEAD ./web`

- Go to the backend folder and click the deploy with Railway button. Fill out the fields including the s3 bucket to deploy as well as the IAM Role with access to S3 buckets.