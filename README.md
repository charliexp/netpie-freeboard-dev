netpie-freeboard
==========

A freeboard with NETPIE datasource and widget plugins.

![netpie-freeboard](https://cloud.githubusercontent.com/assets/7685964/15654676/58211e1c-26c0-11e6-8a53-86c7a2d6de69.jpg)

Installation

git clone https://github.com/netpieio/netpie-freeboard

To use a freeboard, just open the file index.html in any web browser. Under the DATASOURCE section, click ADD to create a new datasource then select NETPIE Microgear and configure as follows:

- **NAME** - the name of the datasource
- **APP ID** - NETPIE App ID
- **KEY** - Microgear Key
- **SECRET** - Secret of the key
- **DEVICE ALIAS** - If needed you can name the datasource as a microgear so it can be reached by a function chat()
- **MICROGEAR REFERENCE** - A reference of the microgear object for a local Javascript. If you enter 'mygear' the microgear object of this datasource will be available as microgear['mygear']
- **SUBSCRIBE TOPICS** - Topics that this datasource will subscribe. Wild cards # and + are allowed. The default value is /# meaning that it subscribes to all topics in this App ID.

![netpie-freeboard2](https://cloud.githubusercontent.com/assets/7685964/15654634/fbe3c096-26bf-11e6-8ab5-4656839b53ad.jpg)

As for the button widget, you can configure it to execute Javascipt codes upon the onClick event. In the picture below the button is configured to send a chat message to the device named *pieslampher* everytime it is clicked. The index 'mg1' is simply the reference of a microgear of a datasource *netpie1* you entered in the datasource configurtion.

![netpie-freeboard3](https://cloud.githubusercontent.com/assets/7685964/15655823/ec23a1f2-26ca-11e6-9968-ee500136b7bc.jpg)
