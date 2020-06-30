# CICD Practice
- Practice release app to google play and app store


# Config Environment Variables
- AWS_ACCESS_KEY_ID: Amazon service access keys
- AWS_S3_BUCKET_NAME: Amazon service S3 bucket name
- AWS_SECRET_ACCESS_KEY: Amazon secret keys
- ENCODED_KEYSTORE_BETA: Keys store for release beta
- ENCODED_KEYSTORE_PROD: Keys store for release prod


# Quickly start

Practice trying building app from Circleci and Github Actions

## Circleci

- Config to build and release with Circleci will config in `.circleci` folder

- All android config build in `CICD/android/fastlane`

- All ios config build in `CICD/ios/fastlane`.
    
    *Notes*: It not work with 
            
    - Free circleci account
    - Invalid developer account

## Github Actions

- Config to build and release with Github Actions will config in `.github` folder

- All android config build in `CICD/android/fastlane`

- All ios config build in `CICD/ios/fastlane`.

# Reference
- [Fastlane](https://docs.fastlane.tools/)
- [Supply](https://docs.fastlane.tools/actions/supply/)
- [Gym](https://docs.fastlane.tools/actions/gym/)

- [Circleci](https://circleci.com/)
- [Github Actions](https://github.com/features/actions)


- My experiences when build app with Circleci and Github actions(Run Test and build android app on same source code)

|                                     | Circleci       | Github actions|
| :---                                |    :----:      |          ---: |
| Duration(Tested build Android)      | ~4m 21s        |  ~4m 23s       |
| Support OS(FREE account)            | Linux, Windows | Ubuntu, MacOS, Windows |
| Support cache                       | Yes            | Yes |
| Syntax template                     | YAML           | YAML |
| Tracking events to trigger building | Push           | Push or pull request |