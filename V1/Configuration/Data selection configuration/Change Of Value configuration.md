---
uid: BACnetCOVConfiguration
---

# Change Of Value (COV) configuration

## Overview

CoV or Change of Value is one of two available data collection modes for the adapter. For supported BACnet devices (i.e. for devices whose Device Configuration's ServicesSupported includes SubscribeCoV and/or SubscribeCoVProperty) users can choose to enable CoV collection. CoV is a subscription-based data collection mode, where the device will "push" new data when the value changes. CoV is generally preferred when available, as it tends to improve performance and decrease network usage.

## Usage 

To enable CoV for a specified data selection item, change the DataCollectionMode to SubscribeCoV or SubscribeCoVProperty. Optionally, a CoVIncrement can also be specified on the data selection item to specify a minimum amount that the value must change in order to prompt the new value to be sent.