# VCF Executive Cost Dashboard

This repository contains the custom view and dashboard used in the article:

https://devynharrington.com/vcf/creating-a-custom-executive-cost-report/

The dashboard provides a simple executive view of VM cost metrics in VMware Aria Operations / VCF Operations.

## Contents

executive-vm-cost-detail.xml  
Custom VM cost view used as the dashboard data source

executive-cost-dashboard.json  
Executive cost dashboard layout

## Import Instructions

1. Import the view first:

Dashboards and Reports → Views → Import  
Select **executive-vm-cost-detail.xml**

2. Import the dashboard:

Dashboards → Manage Dashboards → Import  
Select **executive-cost-dashboard.json**

## Notes

The dashboard expects VMware cost metrics such as:

- cost|monthlyTotalCost
- cost|monthlyProjectedCost
- cost|effectiveDailyCost

These metrics are available when cost calculations are enabled in Aria Operations.
