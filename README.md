# Pegasus Victim Database
Granitt began tracking details about victims of NSO's Pegasus spyware following the publication of the [Pegasus Project](https://forbiddenstories.org/case/the-pegasus-project/) in the summer of 2021. This database is focused on individuals and small groups of people, so you won't find single entries for the "1,400 mobile phones and devices" targeted [through WhatsApp](https://storage.courtlistener.com/recap/gov.uscourts.cand.350613/gov.uscourts.cand.350613.1.0_3.pdf) or "15,000 individuals" [selected](https://www.theguardian.com/news/2021/jul/19/fifty-people-close-mexico-president-amlo-among-potential-targets-nso-clients) for surveillance in Mexico. The goal is to make the records as comprehensive as possible by manually collecting and sorting publicly available information. The database is updated regularly as more information becomes available.

## How to view the data

To view the data, you can:

* Click on the `.csv` file above to view the data right here on GitHub
* Download a `.zip` file by clicking the green `Code`-button, then view it using Microsoft Excel 
* Download a `.zip` file by clicking the green `Code`-button, then import the `.csv` into Google Sheets

## Schema

Each row in the database contains information about one alleged victim. A row may contain information about small groups of victims, such as a team of lawyers or employees at an embassy, until we receive enough details to break it down further.

| **Field**           | Description                                     | Type   | Example value |
| ------------------- | ----------------------------------------------- | ------ | ------------- |
| `name`              | Name of the victim         | String | `John Doe`    |
| `code_name`      | Code name assigned to the victim | String | `USJRN1` |
| `role`              | Victim's role at the time | String | `Journalist`  |
| `organization`      | Victim's organization at the time | String | `El Faro`     |
| `occurred`          | Year the case occurred | String  | `2018` |
| `disclosed` | Year the case was disclosed | String | `2020` |
| `disclosed_by`      | Who the case was disclosed by | String  | `Citizen Lab` |
| `forensics_by` | Who did the analysis/forensics | String | `Lookout` |
| `pegasus_project`   | If the victim was named by the Pegasus Project | Boolean | `TRUE` |
| `apple_warning` | If Apple sent a warning | Boolean | `TRUE` |
| `device_type`       | Type of device | String | `iPhone`   |
| `attack_attempted` | If an attack was attempted | Boolean | `TRUE`  |
| `attack_successful` | If an attack was successful | Boolean | `FALSE` |
| `attack_vector` | How the spyware was delivered | String | `WhatsApp` |
| `exploit_name`      | Name of the exploit used | String | `KISMET`     |
| `first_activity`    | Date of first spyware activity | String | `2018-06-02` |
| `last_activity`     | Date of last spyware activity | String | `2018-07-22` |
| `operator`  | Country operating the spyware | String | `Mexico` |
| `sources`  | List of sources    | String | `granitt.io` |

## The Pegasus Project
The [Pegasus Project](https://forbiddenstories.org/case/the-pegasus-project/) was a large-scale investigation into the use of NSO's Pegasus spyware, coordinated by Forbidden Stories with technical support from Amnesty International. At the center of the investigation was a leaked list of 50,000 phone numbers said to have been selected for surveillance by NSO's customers since 2016. Forbidden Stories and Amnesty International shared the data with [15 media partners](https://forbiddenstories.org/about-the-pegasus-project/), including the Guardian and the Washington Post. Due to the sheer number of potential victims disclosed by the investigation, this database may contain some discrepancies and duplicate entries. 

## How to contribute

We welcome assistance in making the data as complete as possible. Please reach out with any questions, feedback, updated or missing information, corrections, or requests for new fields. You can open an issue in this repository, or email runa@granitt.io. 

## Licensing

The data is published under an Attribution-NonCommercial-ShareAlike 4.0 International CC BY-NC-SA 4.0 license.

## About Granitt

Granitt was founded by Runa Sandvik with the goal of securing journalists and at-risk people around the world. To learn more about our work, see [this TechCrunch interview](https://techcrunch.com/2022/07/15/granitt-journalist-security/) from July 2022.
