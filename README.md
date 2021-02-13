#Opencart-Khipu integration

## Use khipu as a means of payment

This plugin offers integration of the e-commerce system [opencart] (http://www.opencart.com/) with [khipu] (https://khipu.com).
When installed it allows customers to pay using * Simplified transfer * (using the payment terminal) or with * Normal electronic transfer *.
In the portal administration you can define whether both options or only one will be available.

## Installation

You can review an [online guide] (https://khipu.com/page/opencart) on how to install this plugin.

Before activating the khipu extension, you must execute the following steps:

- Create the currency "Chilean Peso" with code CLP.
- Configure your site to use this default currency.

Then you must go to the extensions configuration and activate _Simplified transfer_ and / or _Normal electronic transfer_.

In the configuration of each extension you must include your * collector id * and your * collector key *. You can get these from
the options of your collection account in the khipu portal.

## Package the extension

This extension uses [lib-php] (https://github.com/khipu/lib-php) for communication with khipu. Before packing it is necessary that
update the project submodules by executing:

$ git submodule update --init

Then you must run the shell-script that is included:

$ ./package.sh

After this, the _dist / khipu.ocmod.zip_ file is generated.

## How to report problems or help development

The official site for this extension is its [page on github.com] (https://github.com/khipu/opencart-khipu). If you wish
Report bugs, review the source code or help us improve it, you can use the ticketing and pull-requests system. Any help is welcome.

## GPL license

This plugin is distributed under the terms of the GPL version 3 license. You can read the license.txt file with the license details. 
