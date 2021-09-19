# Membership Renewal Limits Extension

A CiviCRM extension allowing restrictions on when memberships can be renewed.

The extension is licensed under [AGPL-3.0](LICENSE.txt).

## Requirements

* PHP v7.2+
* CiviCRM 5.42

## Installation (Web UI)

Learn more about installing CiviCRM extensions in the [CiviCRM Sysadmin Guide](https://docs.civicrm.org/sysadmin/en/latest/customize/extensions/).

## Installation (CLI, Zip)

Sysadmins and developers may download the `.zip` file for this extension and
install it with the command-line tool [cv](https://github.com/civicrm/cv).

```bash
cd <extension-dir>
cv dl membership-renewal-limit@https://github.com/lemniscus/membership-renewal-limit/archive/master.zip
```

## Installation (CLI, Git)

Sysadmins and developers may clone the [Git](https://en.wikipedia.org/wiki/Git) repo for this extension and
install it with the command-line tool [cv](https://github.com/civicrm/cv).

```bash
git clone https://github.com/FIXME/membership-renewal-limit.git
cv en membership_renewal_limit
```

## Getting Started

Simply enable the extension. At present, it is not configurable. It will
intercept any Contribution Page submissions which would result in a membership
renewal, and present an error message to the user if the renewal is being 
attempted less than 30 days before the end date of the user's current 
membership.