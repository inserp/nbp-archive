# nbp-archive
A WordPress plugin to collect and view currency rates from Bank of Poland public API. 

## Description

This plugin collect and allow to view historical currency rates from Bank of Poland by using custom Gutenberg Blocks and REST API.

The plugin use Bank of Poland public API for collecting the rates.

Endpoint: https://api.nbp.pl/api/exchangerates/tables/a

Bank of Poland API description and terms of use: https://api.nbp.pl/en.html

After plugin installation your site will provide Bank of Poland historical data using your local database and directly from your domain as REST API service (see FAQ about endpoints).

## Installation
 
1. Upload the plugin folder to your /wp-content/plugins/ folder.
2. Go to the **Plugins** page and activate the plugin.
 
## Frequently Asked Questions
 
## Which API endpoints can I use after installation
### 1. List of currencies rates for available needed date and date before it.

Example: https://your-domain-name.com/wp-json/archive-bnp/v1/date-rates/YYYY-MM-DD/AAA,BBB

Where: YYYY - year; MM-month; DD-day; AAA,BBB -  ISO 4217 currency codes, for example - USD,EUR

### 2. List of rates for needed currency and dates range.

Example: https://your-domain-name.com/wp-json/archive-bnp/v1/currencies-period/YYYY-MM-DD/YYYY-MM-DD/AAA

Where: YYYY - year; MM-month; DD-day; AAA,BBB -  ISO 4217 currency code, for example - USD

## Are any translation available for the plugin?
Plugin support 2 languages: English and Polish.

## Which Gutenberg Blocks can I use after installation
1. **Currency Chart** - show rates for needed currency and dates range as a chart. If you want to have the last available date on the chart always then set Date end parameter far in the future.
2. **Last Rates** - show rates for needed date. Set the date far in the future if you want to show last rates always.
3. **Currency Converter** - allow to calculate any amount in different currencies using last available rates in the table.

## How to uninstall the plugin?
 Simply deactivate and delete the plugin. 
 
## Changelog
**1.0.1**
* Plugin released.
