# Hivebrite Hackathon

## Dust micro service

The goal of our team was to integrate a [Dust](https://dust.tt/) agent in our admin backend interface.
We want to allow our clients to ask questions about our Knowledge Base (Zendesk) to an AI bot accessing our private KB pages.

This micro service:
* Uses Dust [official SDK repository](https://github.com/dust-tt/dust/tree/main/sdks/js)
* Act as a bridge between Frontend code and Dust
  * However, some authentication should be applied here
* Contains the credentials and config to interact with Dust, see config/dust_secrets.example.ts

## Code quality

This was created during a Hackathon.
Do not use this code as it is.
Just an inspiration ;)

## Usage

```
cd hackathon-dust-microservice
cp config/dust_secrets.example.ts config/dust_secrets.ts
# fix the file
npm install
npm run dev
```
-> http://localhost:5000/test?q=ask%20your%20question