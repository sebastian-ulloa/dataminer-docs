---
uid: EPM_6.1.4_D-DOCSIS
---

# EPM 6.1.4 D-DOCSIS - Preview

## New features

#### Fan tray and power supply monitoring added to CCAP visual [ID_33649]

Monitoring of the fan trays and power supply modules has been added to the CCAP visual. The number of power supply modules on the visual will match the number of installed power supplies in that CCAP.

#### 'All' filter option added to table drop-down filters [ID_33739]

An *All* filter option has been added to all table drop-down filters, so that users can clear specific filters without using the *Clear* button, which clears all active filters.

## Changes

### Enhancements

#### CCAP link added to RPD and Node Segment visuals [ID_33645]

A link to the CCAP has been added to the *RPD* and *Node Segment* visuals. In addition, the device symbols in other navigation links throughout the EPM Solution have been adjusted.

#### Improved CM manufacturer info [ID_33646]

The OUI file from which the connectors read the cable modem (CM) manufacturer information has been updated. As this file now has new entries, all CMs will now have a manufacturer associated with them, including those where the manufacturer was previously indicated as *Unknown*.

#### Uniform MAC address throughout EPM Solution [ID_33710]

The MAC address format throughout the EPM Solution and across the different collectors has been made more uniform. The octets in the MAC address are now always separated by a colon. This way, you can now copy a MAC address and search for it throughout EPM, since its format will always be the same.

#### RPD Association page removed from RPD and Node Segment visuals [ID_33736]

The *RPD Association* page has been removed from the *RPD* and *Node Segment* visuals.

#### MLD status removed from Core Leaf visuals [ID_33737]

The MLD status has been removed from the *Core Leaf* visuals.

#### Improved CM MAC search parsing [ID_33738]

CM MAC search parsing has been improved to account for MACs separated by hyphens or using any combination of colon, period, or hyphen to separate the bytes.

#### Removed unnecessary table headers [ID_33894]

Table headers that were unnecessary or not useful to the user, such as average or percent values that disregard the calculation weight, have been removed.

#### Dashboards: "Last Updated" changed to "Last Overall System Update" [ID_33895]

To make it more clear where the data in EPM dashboards comes from, the *Last Updated* label in the dashboards has been changed to *Last Overall System Update*.

#### Topology page removed from Hub visual overview [ID_33896]

To prevent issues where too many RPAs are present and it becomes difficult to show them, the *Topology* page has been removed from the Hub visual overview.

#### Parameter access levels adjusted [ID_33897]

The access levels of write parameters in the EPM connectors have been adjusted so that regular operators will not have access to them. The write parameters now require access level 1, whereas operators only have access level 3.

#### Additional status information in visual overview [ID_34069]

<!-- For fix part of RN, see fixes -->

In the *RPD Details*, a link has been added to the *Partial OFDM CM* KPI. In addition, new columns with the *DS Service Status*, *US Service Status*, and *OFDM Status* have been added to the CM tables in visual overview.

#### Skyline CCAP Platform EPM visual overview improvements [ID_34070]

On the *CCAP/CM* page of the *Skyline CCAP Platform* EPM visual overview, a new status filter box has been added. It allows you to select the option *All* to clear the filter, and the option *Not Operational* to filter out all CMs that are considered offline. In addition, links on the *CCAP/Overview* page have been updated to filter on status instead of MAC state.

#### Performance improvement through SLElement utilization improvements [ID_34309]

To improve performance, several changes have been implemented to reduce the amount of memory used by the SLElement process. As a result of these, the solution will load faster and be more stable.

These changes include:

- The removal of all unnecessary monitored parameters.
- More efficient buffer cleanup logic.
- Removal of the *Counters History* column in the *CmUpstream* table of the Cox CBR-8 Platform D-DOCSIS connector.

### Fixes

#### Ceeview link on RPD Topology page not working [ID_33612]

On the *RPD Topology* page, it could occur that the Ceeview link did not function correctly.

#### Market utilization filter issue [ID_33647]

In the *Utilization* tab of the Market topology level, when you filtered the DOCSIS QAM and OFDM upstream and downstream utilization using either the "\>=" or the "\<=" filter, it could occur that the other filter continued to be applied in the background, so that the two filters were applied to the table at the same time. Now when a specific filter is selected, only that filter is applied to the table, even if the alternative filter has a value filled in.

#### Temperature graph in RPD dashboard did not show selected time period [ID_33648]

In the RPD dashboard, if a different time period was selected, the graph for the *Temperature* component continued to display the values for the last 24 hours.

#### Incorrect interfaces status in RPA visual overview [ID_33898]

In the visual overview of an RPA element, it could occur that the RPA interfaces status was incorrect.

#### Incorrect OFDM Status [ID_34069]

<!-- For enhancement part of RN, see enhancements -->

Up to now, it could occur that the *OFDM Status* was not correct, as the logic did not properly use the *CM Impaired Channels* table to find out if an impaired channel was an OFDM or QAM channel. The logic has been adjusted. As part of this, the "Active" OFDM status no longer exists, and the "OK" and "Partial" status have been introduced to identify CMs without any impaired OFDM channels and CMs with at least one impaired OFDM channel, respectively.