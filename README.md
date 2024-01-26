# EPP Registrar Module for FOSSBilling (AFNIC)

## Compatibility

This module is designed for use with AFNIC registry - all extensions.

# FOSSBilling Module Installation instructions

## 1. Download and Install FOSSBilling:

Start by downloading the latest version of FOSSBilling from the official website (https://fossbilling.org/). Follow the provided instructions to install it.

## 2. Installation and Configuration of Registrar Adapter:

First, download this repository which contains the AFNIC.php file. After successfully downloading the repository, move the AFNIC.php file into the `[FOSSBilling]/library/Registrar/Adapter` directory.

On lines 311 and 312 you will need to put a hardcoded contact ID  for transfer requests. There is no way currently to pass it via FOSSBilling. Just replace the {{ admin }} and {{ tech }} with the chosen contact ID.

## 3. Activate the Domain Registrar Module:

Within FOSSBilling, go to **System -> Domain Registration -> New Domain Registrar** and activate the new domain registrar.

## 4. Registrar Configuration:

Next, head to the "**Registrars**" tab. Here, you'll need to enter your specific configuration details, including the path to your SSL certificate and key.

## 5. Adding a New TLD:

Finally, add a new Top Level Domain (TLD) using your module from the "**New Top Level Domain**" tab. Make sure to configure all necessary details, such as pricing, within this tab.
