# Changelog
## [2.26.1](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.26.1) (2020-03-19)
   - Removes bank_account_verified parameter to Account response entity
   - Removes optional bank_account_verified query parameter to /accounts/find

## [2.26.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.26.0) (2020-03-15)
   - Adds on_behalf_option parameter to /reference/conversion_dates
   - Adds bank_account_verified parameter to Account response entity
   - Adds optional bank_account_verified query parameter to /accounts/find

## [2.25.1](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.25.1) (2020-02-18)
   - Adds new next_day conversion date option for ConversionDates endpoint

## [2.24.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.24.0) (2020-02-03)
   - Removes partner_status field in conversions response
   
## [2.23.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.23.0) (2020-12-23)
   - Adds terms_and_conditions_accepted and agent_or_reliance parameters to account details 
 
## [2.22.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.20.0) (2020-12-15)
   - Updates the default value of the spread table in accounts/create endpoint.
   - Adds offline_conversion_dates to response from reference/conversion_dates endpoint.
   - Deprecate ibans/find 
   - Deprecate virtual_accounts/find 
   - Deprecate partner_status field in conversions response

## [2.20.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.20.0) (2020-11-25)
   - Removes purpose_code parameter from payments find.
   - Removes all settlement model endpoints.
   - Adds new error codes for canceling a transfer.

## [2.19.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.19.0) (2020-10-29)
   - Updates create beneficiary endpoint to differentiate between company and individual identification.
   - Updates documentation for conversion endpoints.
   - Adds 'cancelled' as possible option for 'status' parameter on find transfers.
   - Adds description for sender tag in get sender details.
   - Update the endpoint /v2/reference/beneficiary_required_details making currency, bank_account_country, 
   beneficiary_country required rather than optional          

## [2.18.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.18.0) (2020-10-15)
   - Adds transfers/cancel endpoint
   - Adds unsupported_account error response to payments/crate
   
## [2.17.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.17.0) (2020-10-01)
   - Updates ConversionDates definition.
   - Updates 'Create Conversion' API to reflect UTC for conversion_date instead of ISO 8601 format.
      
## [2.16.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.16.0) (2020-09-15)
   - Adds payments/validate endpoint
   - Updated the names of routing_code_type and routing_code_value on beneficiaries/find
   - Sets postal_code as optional on accounts/create

## [2.15.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.15.0) (2020-09-11)
   - Removed "awaiting_balance" from list of possible status for find payment endpoint
   - Changed contact status from enabled and disabled to enabled and not_enabled
   - Update the description for field 'as_at_date' so that the example doesn't specify the timezone offset 

## [2.14.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.14.0) (2020-06-26)
   - Adds optimize_liquidity_conversion_date to reference/conversion_dates response
   - Removes account_id and contact_id parameters from report_requests/find endpoint 
   - Adds payments tracking_info endpoint

## [2.13.1](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.13.1) (2020-05-18)
   - Updates amount limit error message on withdrawal_accounts pull_funds

## [2.13.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.13.0) (2020-05-04)
   - Adds Conversion date preference parameter to /v2/rates/detailed and /v2/conversions/create

## [2.12.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.12.0) (2020-03-24)
   - Adds /payments/assign_payment_fee endpoint
   - Adds /payments/payment_fees endpoint
   - Adds /payments/unassign_payment_fee endpoint
   - Adds payment_fee_id and payment_fee_name to PaymentFeeRule response definition

## [2.11.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.11.0) (2020-03-09)
   - Adds top_up_margin endpoint definition

## [2.10.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.10.0) (2020-01-22)
   - Makes currency required for /funding_accounts/find 
   - Adds "margin" to action enum in transactions find
   - Adds awaiting_balance to status enum of find payments 
   - Adds unsupported_beneficiary_country_code error response to payments/create
   - Updates the routing_code parameters in Funding Accounts object

## [2.9.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.9.0) (2019-10-21)
   - Updates Payments endpoints for payment fee parameters
   - Updates transaction find endpoint for payment_fee action
   
## [2.8.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.8.0) (2019-10-11)
   - Updates error response on bank_details endpoint for invalid cnaps
   - Adds find funding accounts end point
   - Adds get payment level fees endpoint
   - Adds get quote payment fee endpoint
   
## [2.7.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.7.0) (2019-08-01)
   - Adds additional supported identifier types to bank details end point
   - Adds contacts generate_hmac_key end point
   - Fixes duplicated operation Id for Pull Funds From Withdrawal Account

## [2.6.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.6.0) (2019-06-25)
   - Adds find withdrawal_accounts end point
   - Adds pull_funds from withdrawal_accounts end point
   - Adds bic_swift option to identifier_type of bank_details end point

## [2.5.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.5.0) (2019-04-25)
   - Adds get bank_details endpoint
   - Adds beneficiary_external_reference parameter to beneficiaries create and update endpoints
   - Fixes missing parameters in BeneficiaryRequirements definition

## [2.4.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.4.0) (2019-04-25)
   - Removes support for deprecated VANS and IBANS operations
   - Deprecates all settlement operations
   - Adds action_type deposit_refund to transaction find operation
   - Updates error codes on beneficiaries/find operation
   - Fixes type of deposit_required and deposit_amount in Conversion model
   - Fixes indentation of default value for payment_types parameter
   - Fixes description of id parameter on transactions/sender operation


## [2.3.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.3.0b) (2019-03-11)
   - Adds currency as an optional field in the 'Get Requirements for Payers' API
   - Adds beneficiary_external_reference as an optional field in the 'Find Beneficiaries' API
   - Bugfix to 'Create Beneficiary' beneficiary_identification_type enum list
   - Bugfix to 'Find Payments' charge_type parameter 'in' type
    
    
## [2.2.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.2.0) (2019-02-19)
   - Adds enum and default values for scope parmeter on find-ibans and find-vans
   - Adds missing actions to the enum of the action parameter of transactions/find
   - Updates documentation for transactions/find, payments/find and payments/create
   - Add Payment Charge Settings
   - Create beneficiary enum list fix
   - Fix Beneficiary Payment Type Defaults
   - Adds get payment delivery date to api definition



## [2.1.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.1.0) (2019-02-05)
   - Fixes documentation of *Get Payer Requirements*
   - Documents 403 Error
   - Adds wire_routing_code to VANS Definition


## [2.0.0](https://github.com/CurrencyCloud/currencycloud-swagger/releases/tag/rel-2.0.0) (2109-01-30)


## Initial Release (2018-05-16)
