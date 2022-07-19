# qtc_ViewExternal
VF page with instructions to create CPQ Custom Action in configurator that displays the JSON payload in a given Bundle. Useful for troubleshooting governor limits in the configurator. 

Here are the steps to implement the View External custom action in any org: 
  1. Create custom VF page (code attached) named qtc_ExtConfig. Note: there is no controller needed. 
  2. Navigate to Installed Packages | Salesforce CPQ | Configure | Additional Settings --> set the External Configurator URL to *InstanceName.visualforce.com/apex/qtc_ExtConfig
  3. Navigate to Setup | Session Settings --> ensure the "Enable clickjack protection for customer Visualforce pages with headers disabled" checkbox is UNCHECKED
  4. Navigate to Bundle product we want to evaluate and check the Externally Configurable checkbox
  5. Create a new Custom Action with the values shown in the image below: 
