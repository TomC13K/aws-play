# Project to test localstack (AWS) features 


## Initialization

### NodeJS TS project

```bash
npm init -y
npm install --save-dev typescript
npx tsc --init
npm install --save-dev eslint
npx eslint --init
```

### Express Framework
```bash
npm install --save express@4.17.1
npm install -save-dev @types/express@4.17.1
```

### AWS-SDK

change from V2 to V3 now can only install individual libraries for specific services

https://docs.aws.amazon.com/AWSJavaScriptSDK/v3/latest/

```bash
npm install @aws-sdk/client-lambda
```

## Localstack, terraform
```bash
# Install localstack CLI
brew install localstack/tap/localstack-cli

# Install terraformlocal & terraform
brew install terraform
brew install terraform-local

# use localstack in the project
localstack config validate
docker compose up -d

## terraform
tflocal init
tflocal plan
tflocal apply
```