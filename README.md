
# Installation
1. Run `git clone --recurse-submodules git@gitlab.com:ev-charging-solutions/altium-lcsc-lib.git`
2. In ODBC Connector (you can download it [here](https://dev.mysql.com/downloads/connector/odbc/)), click on **Add** button, select **MySQL ODBC 8.0 Unicode Driver**, fill in information about the database along with data source name and click **OK**.
3. In your project, add **Database_Lib2.DbLib** and open it.
4. Click on **Build** button.
5. In the Provider tab select **Microsoft OLE Provider for ODBC Drivers**.
6. In the Connection tab, in **Use data source name**, find the data source name from step 2 and select the initial catalog as the database in use.
7. **\*optional\*** If you are looking at the components panel and can see different categories/views, but you cannot see any components in any view, try restarting the application.

## How to generate new components?
1. Go to **altium-jlc-parser** folder inside the cloned repo.
2. Create **.env** file and inside of it set these variables: 
**DB_USER, DB_PASSWORD, DB_ADDRESS, DB_PORT, DB_NAME** 

3. Go to **config** folder and inside of **filter.json** set parameters **enabled**, **minimal_stock**, **basic**, **extended**, **manufacturers** and **lcsc_numbers**
 
> Note: you can see new added categories inside of the **Change Log**, or see every category inside of **mapping.json** file.
4. Run ```main.py```  


# Change Log
## Release v1.0 
— Added category: **Resistors** <br>
— Added subcategory: **Chip Resistor -  Surface Mount** (Resistors) <br>
— Added  category: **Capacitors** <br>
— Added subcategory: **Multilayer Ceramic  Capacitors MLCC - SMD-SMT** (Capacitors)