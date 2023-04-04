# Getting Started

Welcome to your new project.

It contains these folders and files, following our recommended project layout:

File or Folder | Purpose
---------|----------
`app/` | content for UI frontends goes here
`db/` | your domain models and data go here
`srv/` | your service models and code go here
`package.json` | project metadata and configuration
`readme.md` | this getting started guide


## Next Steps

- Open a new terminal and run `cds watch` 
- (in VS Code simply choose _**Terminal** > Run Task > cds watch_)
- Start adding content, for example, a [db/schema.cds](db/schema.cds).


## Learn More

Learn more at https://cap.cloud.sap/docs/get-started/.

## Database Configuration Notes

CREATE REMOTE SOURCE "RS_PBH"

ADAPTER "hanaodbc"

CONFIGURATION '<?xml version="1.0" encoding="UTF-8"?><ConnectionProperties name="connectionproperties"><PropertyEntry name="adapterversion">1.0</PropertyEntry><PropertyEntry name="connectionmode">adapterproperties</PropertyEntry><PropertyEntry name="driver">libodbcHDB.so</PropertyEntry><PropertyEntry name="server">pbh</PropertyEntry><PropertyEntry name="port">30</PropertyEntry><PropertyEntry name="dml_mode">readwrite</PropertyEntry><PropertyEntry name="extraadapterproperties">use_haas_socks_proxy=true;scc_location_id=CCJDZ</PropertyEntry></ConnectionProperties>'

WITH CREDENTIAL TYPE 'PASSWORD' USING 'user=????????;password=????????';


REMOTE_SOURCE_ROLE


## UPS JSON File

{
    "user": "??????",
    "password": "??????",
    "tags": [
        "hana"
    ],
    "driver": "com.sap.db.jdbc.Driver",
    "endpoint": "https://api.cf.us10.hana.ondemand.com",
    "host": "????.hana.trial-us10.hanacloud.ondemand.com",
    "port": "443",
    "encrypt": true,
    "validate_certificate": false,
    "schema": "??????"
}



