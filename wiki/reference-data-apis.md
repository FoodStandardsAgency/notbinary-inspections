## API prototyping

A key part of the technology theme running through the discovery and prototyping work for the inspections service is separating system responsibilities into clear areas of data ownership, processing and storage. Along with this, ensuring each area offers access to the data it owns is key to creating an overall service in which parts collaborate and support each other, data is stored once, available to be used many times and accessed at source by default.

Current industry practice for supporting automated data access and exchange between systems and system components is via Application Programming Interfaces (APIs). This approach focuses on making data and/or functions available, accessible and understandable by other components of the system - i.e. a "user interface", where the user is a machine.

In order to test out this principle in practice, "code sketches" were produced to make it possible to visualise what direct system-to-system access to data could look like. These sketch prototypes are focused on illustrating, in a simple way, what APIs could look like and how these might support other parts of the inspection service in delivering their area of responsibility.

To be clear, they aren't intended to be comprehensive, accurate or production-quality and don't cover all the features that would be needed. The intent is to visualise, in a concrete way, the art of the possible, and further the conversation about the role of data in facilitating an integrated service.

### API sketches

At the time of writing, the following API sketches are available via an [API index page](https://fsa-reference-data.herokuapp.com/):

 * [Site types](https://fsa-reference-data.herokuapp.com/site-types): the types of site within an establishment, for example Red Meat Slaughterhouse (RSL)
 * [Activity codes](https://fsa-reference-data.herokuapp.com/activity-codes): The list of activities that can be performed at meat processing establishments, such as Inspection (INSP)
 * [Rate codes](https://fsa-reference-data.herokuapp.com/rate-codes): the rates at which inspection time is charged, for example Normal working hours (00)
 * [Establishment information](https://fsa-reference-data.herokuapp.com/establishments): this serves data from a csv file from the [fsadata repo on Github](https://github.com/fsadata/approved-food-establishments/tree/gh-pages/data). (NB this operational rather than reference data)

### API code and data

Initially each API was built using individial code that read data from a CSV file embedded in the code. The aim here was to provide a straightforward format for the data and process for updating it. 

This model was improved on to further simplify the process, using a [codebas developed for the Urban Flows hackathon](https://urban-flows-api.herokuapp.com/), available in the [data-bear repository on Github](https://github.com/davidcarboni/data-bear). This code is able to read a collection of spreadsheets from an open Google Drive folder and serve each as an API.

The folder containing the spreadsheets of data for the APIs above can be found at the following link: https://drive.google.com/drive/folders/1lTMzmb-N4F3nznDY5eV003O8NomPTYBg