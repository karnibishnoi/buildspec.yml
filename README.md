version 0.2

phases:
  build:
    commands:
    - echo "This is build phase... Zipping my webpage"

    post_build:
      commands:
      - echo "Deployed to s3"
 artifacts:
   files:
   - '**/*'
