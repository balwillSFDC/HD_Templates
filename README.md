HD Build instruction

- Build package in scratch org and package as json
- Replace references to Campaign Name with {{mcpm:CampaignName}}
- Replace references to Touchpoints with {{mcpm:Touchpoint1}} (or whatever # touchpoint)
- Replace UpdateContact Event value references to reference Event Def Key
- Replace EventDefinitionKey value to be exact
  - `"eventDefinitionKey": "eventDef{{mcpm#/random/{{mcpm:CampaignName | label:Campaign Name}}_{{mcpm:Touchpoint2 | label:Touchpoint 2 Name}}_UAT}}""` should be `"eventDefinitionKey": "{{mcpm:CampaignName | label:Campaign Name}}_{{mcpm:Touchpoint1 | label:Touchpoint 1 Name}}_UAT"`
