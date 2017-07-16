
Registry service requires 

- 'my-company-configuration-backingservice' (on staging and production)

You can create it manually on PWS, or by running script:

```
cf api https://api.run.pivotal.io
cf auth idugalic@gmail.com $CF_PASSWORD

cf target -o idugalic -s Stage
cf create-user-provided-service my-company-configuration-backingservice -p '{"uri":"https://stage-my-company-configuration-backingservice.cfapps.io"}'

cf t -s Prod
cf create-user-provided-service my-company-configuration-backingservice -p '{"uri":"https://prod-my-company-configuration-backingservice.cfapps.io"}'

```