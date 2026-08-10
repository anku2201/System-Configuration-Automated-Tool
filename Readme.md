
# Auto Configuration Setup


This is a tool that automates the configuration of the IDEAL application. It can be used to configure both the technical and functional aspects of the application.

**Prerequisites**

* **Node.js**
* **Git**

**Instructions**

1. Clone the repository:


```
$ git clone https://gitlab.credenceanalytics.com/apac-development-team/interface/common-module/system-configuration-automation.git
```


2. Go to the `config` folder and open the `config.json` file. This is where you will need to specify the configuration for the tool.


```
$ cd system-configuration-automation/config
$ open config.json
```


The following are the required parameters:

* **`sourcepath`** : The path to the source code for the IDEAL application.
* **`wildfly_folder`** : The name of the WildFly/JBoss folder.
* **`war_folder`** : The name of the WAR folder.
* **`oracledb`** : An array of objects that define the Oracle database connections.
* **`JAVA_PATH`** : The path to the Java installation.
* **`quname`** : The username for connecting to the message queue.
* **`qpwd`** : The password for the message queue user.
* **`metabase`** : An object that defines the Metabase configuration.
* **`client_name`** : The name of the client.
* **`client_address`** : The address of the client's location.
* **`lcy_curr_main`** : The main local currency.
* **`gcy_curr_main`** : The main global currency.
* **`defaultDealLocationName`** : The default location name for deals.
* **`defaultDealLocationCode`** : The default location code for deals.
* **`default_payment_mode`** : The default payment mode.
* **`Default_Delivery_Location`** : The default delivery location.
* **`domesticcurrency`** : The domestic currency.
* **`globalcurrency`** : The global currency.
* **`groupcurrency`** : The group currency.



**Running the tool**

Once you have configured the `config.json` file, you can run the tool by going to the `run` folder and running the following commands:

**For Linux systems**

* For technical configuration:

```
$ cd system-configuration-automation/run
$ sh run_techfile.sh
$ sh run_techdb.sh
```

* For functional configuration:

```
$ sh run_funcfile.sh
$ sh run_funcdb.sh
```

**For Windows systems**

 Go to the `Run` folder.
* For technical configuration:

--- Double click on the `run_techfile.bat` file.
--- Double click on the `run_techdb.bat` file.

* For functional configuration

--- Double click on the `run_funcfile.bat` file.
--- Double click on the `run_funcdb.bat` file.


-----------------------------
**Notes**
**The tool will create logs in the `log` folder and will also create backups of the previous files in the `filebackup` folder.**

If you have any problems running the tool, please check the following:

* Make sure that you have the required prerequisites installed.
* Make sure that the `config.json` file is properly formatted.
* Make sure that the paths in the `config.json` file are correct.
* If you are still having problems, please contact the development team.

