
# Modify DB
update chain set chain_name="Codemason", chain_code3="CMN" where chain_name ="Dash";

# abe-my.conf
dbtype MySQLdb
connect-args {"user":"abe","db":"abe","passwd":"PASSWORD"}
upgrade
port 2750
datadir += [{
            "dirname": "/data/dev1",
            "chain":   "Codemason",
            "code3":   "CMN",
            "address_version": "o" }]