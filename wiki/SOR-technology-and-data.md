## Technology and data: SOR

SORs are currently entered into and held by a K2 Forms application. This was built several years ago to digitise an existing spreadsheet process.

The current implementation suffers from slow page load times and the user flow is not optimised, meaning it takes longer than necessary to enter an SOR.

### Current technology

 * K2 Forms

The current system is implemented using the K2 Forms engine. K2 provides additional capabilities that are not currently in use by SOR so there are additional options available within the existing technology that could be used to implement a redesigned process and user experience.

### Data considerations

The SOR system does not currently offer API access to the data it holds. Providing API access would open the door for integration to enable downstream processes (such as Rotas and Timesheeting) to access SOR data and make use of it to facilitate their own part of the overall service.

A significant proportion of the information required to complete the SOR processes is held in the Single Information Repository (SIR) database. For example information about approved establishments and reference data such as site types and activity codes. It would advantageous if SOR can be integrated with enabling applications and reference data in their current state and/or as-and-when these are modernised.

The aim would be to enable each type of data to be accessed from a single authoritative source. This could avoid duplication, manual effort to move data between systems and possible discrepancy (especially around times when changes are made). The technology underpinning the overall inspection service can be visualised as a network of inter-related components, each with a clear, focused single function that meets needs of dependent systems. For example, Activities and Establishments could be two separate systems that provide data via API to SOR. In turn, SOR could provide data via API to Rotas and Timesheets.

### Recommendations

The SOR system is understood to have been implemented as a tactical solution to digitise an existing paper process. Whilst the solution is not ideal, it has been sufficiently fit-for-purpose to enable the delivery of meat plant inspections.

There is now an opportunity to review the existing system. The following are key areas of opportunity:

 * Improve the user experience to facilitate efficient development, review and adjustment of SOR agreements
 * Integrate SOR with data sources that can help improve user experience, such as information about plants, sites, roles and activity codes
 * Enable SOR to expose agreement data in such a way that this could be used to support improved rota and timesheeting processes
 * The current SOR implementation is primarily driven by the approval number of a plant. It would be helpful to be able to see which agreement is current andh where an agreement is draft, seasonal or superseded
 * Enable SOR data to feed in to improved reporting and enable FSA to continuously improve field operations