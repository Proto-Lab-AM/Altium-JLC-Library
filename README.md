# Installation
1. In the beginning, run `git clone --recurse-submodules git@gitlab.com:ev-charging-solutions/altium-lcsc-lib.git`
2. In ODBC Connector, click on **Add** button, select **MySQL ODBC 8.0 Unicode Driver**, fill in information about your database along with data source name and click **OK**  
3. In your project, add **Database_Lib2.DbLib** and open it
4. Click on **Build** button
5. In the Provider tab select **Microsoft OLE Provider for ODBC Drivers**
6. In the Connection tab, in **Use data source name**, find your data source name from step 2 and select the initial catalog as the database in use.

## How to generate new components?
1. Go to **altium-jlc-parser** folder inside the cloned repo.
2. Create **.env** file and inside of it set these variables: 
**DB_USER, DB_PASSWORD, DB_ADDRESS, DB_PORT, DB_NAME** 
3. Go to **config** folder and inside of **filter.json** add available categories and subcategories. You can also choose specific parts based on **mfr_part** and **lcsc_part**
 
> Note: you can see new added categories inside of the **Change Log**, or see every category inside of **mapping.json** file.
4. Run ```main.py```  



# Changelog
— Added category: **Resistors**
— Added subcategory: **Chip Resistor - Surface Mount** (Resistors)
— Added  category: **Capacitors**
— Added subcategory: **Multilayer Ceramic Capacitors MLCC - SMD-SMT** (Capacitors)
