# dwp-job-seekers-allowance
Number, and percent, of people in Edinburgh claiming Job Seeker's Allowance by gender and age.

JSA replaced Unemployment Benefit and Income Support for unemployed people in October 1996. It is payable to people under pensionable age who are available for, and actively seeking work with some exclusions. There are contribution-based and income-based routes of entry to JSA. Income-based JSA is similar to Income Support and the majority of JSA recipients are expected to qualify through this route.

Data shown here are derived from a 100% data source; the Work and Pensions Longitudinal Study (WPLS) which is not subject to any sampling error. The dataset provides counts of total claimants and breakdowns by age and gender from a snapshot in time and will therefore exclude a small number of clerically held cases.

The snapshots are taken at quarterly intervals at the end of February (Q1), May (Q2), August (Q3) and November (Q4). The scans from this source do not have accurate markers to indicate receipt of income based JSA or not. A very small number of claimants who have an unknown age or gender are included within the area total but excluded from the age and gender breakdowns as they pose a small disclosure risk. Due to low numbers it has not been possible to give information on duration on benefit, but this can be found via the claimant count on NOMIS.

The data in the WPLS datasets are not directly comparable to the annual individual level data previously released as they were a single snapshot at a point in time and did not reflect late notifications and removals from the systems. Claim rates are calculated using the working age population (males aged 16-64 and females aged 16-59) from the small area population estimates published by the National Records of Scotland.  Figures based on the Data Zones 2001.

Source: Department for Work and Pensions. http://statistics.gov.scot/data/job-seekers-allowance

## License

Data is licensed under the Open Government License: http://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/

## Requirements

- NodeJS
- npm

## Installation

Clone the repository

```
git clone https://github.com/EdinburghCityScope/dwp-job-seekers-allowance.git
```

Install npm dependencies

```
cd dwp-job-seekers-allowance
npm install
```

Run the API (from the dwp-job-seekers-allowance directory)

```
node .
```

Converting the extracted data into loopback data.

```
node scripts/featureCollectionToLoopbackJson.js
```

Re-build data files from the statistics.gov.scot API

```
node scripts/build-data.js
```
