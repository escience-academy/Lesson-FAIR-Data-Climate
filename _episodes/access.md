---
title: "Access to the data"
teaching: 10
exercises: 15
questions:
- "What is meant by 'accessibility'?"
- "What are relevant data repositories in climate science?"
- "How to choose a data repository?"
objectives:
- "Identify suitable repositories to make your research data acessible."
- "Plan access to the data in a data management plan."
keypoints:
- "Accessible does not mean open without constraint."
- "Metadata can still be accessible, even if the data itself is not (anymore)."
- "EU-funded projects are expected to make generated data accessible to the public."
---


## What is access to data?

Accessibility addresses the *A* in the FAIR principles. Once the user finds the required data, she/he needs to know how can they be accessed, possibly including authentication and authorisation. Accessible data objects can be obtained by humans and machines upon appropriate authorisation and through a well-defined and universally implementable protocol. In other words, anyone with a computer and an internet connection should be able to access at least the metadata.

> ## This is what [go-FAIR.org](https://go-fair.org/principles) has to say about Accessible
> - A1. (Meta)data are retrievable by their identifier using a standardised communications protocol
> - A1.1 The protocol is open, free, and universally implementable
> - A1.2 The protocol allows for an authentication and authorisation procedure, where necessary
> - A2. Metadata are accessible, even when the data are no longer available
{: .checklist}

> ## Accessible does not mean open without constraint
> Accessibility means that the human or machine is provided - through metadata - with the precise conditions by which the data are accessible and that the mechanisms and technical protocols for data access are implemented such that the data and/or metadata can be accessed and used at scale, by machines, across the web.
{: .callout}

## FAIRness in climate science

Although FAIRness in climate science is advancing and some clearly accessible repositories exist, it is still also common practice to only make a dataset accessible via the project website. Because projects do not last for ever, some of these websites are not maintained, resulting in inaccessible datasets.

Next to large-scale general-use repositories such as [Zenodo](https://zenodo.org/), there are also several domain-specific repositories. You may be familiar with [ESGF](https://esgf.llnl.gov/), [CDS](https://cds.climate.copernicus.eu), or [Climate4Impact](https://climate4impact.eu).

> ## Stages of accessibility
>
> You submitted a paper, and the reviewer asks you to make your data accessible. You consider your options,
>
> 1. You make a note in your paper that data can be requested by sending you an email
> 2. You provide the data as supplementary information to your paper
> 3. You upload the data to some cloud storage and put a shareable link in your paper
> 4. You upload the data to a university drive and request a DOI from the library
> 5. You upload the data to a generic repository such as zenodo
> 6. You upload the data to a domain-specific repository such as [Hydroshare](https://www.hydroshare.org/)
>
> Describe which of these are adhering to the [FAIR principles](https://www.go-fair.org/fair-principles/), focusing on the findability and accessibility criteria.
>
>> ## Solution
>> <table style="width:50%">
>>   <thead>
>>     <tr>
>>       <th></th>
>>       <th>F1</th>
>>       <th>F2</th>
>>       <th>F3</th>
>>       <th>F4</th>
>>       <th>A1</th>
>>       <th>A1.1</th>
>>       <th>A1.2</th>
>>       <th>A2</th>
>>       <th>Verdict</th>
>>     </tr>
>>   </thead>
>>   <tbody>
>>     <tr>
>>       <td>1.</td>
>>       <td>😢❌</td>
>>       <td>😢❌</td>
>>       <td>😢❌</td>
>>       <td>😢❌</td>
>>       <td>😢❌</td>
>>       <td>😢❌</td>
>>       <td>😢❌</td>
>>       <td>😢❌</td>
>>       <td>Hard to find and difficult to access. </td>
>>     </tr>
>>     <tr>
>>       <td>2.</td>
>>       <td>🤔❓</td>
>>       <td>🤔❓</td>
>>       <td>😢❌</td>
>>       <td>😢❌</td>
>>       <td>😢❌</td>
>>       <td>🤔❓</td>
>>       <td>🤔❓</td>
>>       <td>😢❌</td>
>>       <td>Data may be found indirectly through the papers DOI, but there is no clear access protocol.</td>
>>     </tr>
>>     <tr>
>>       <td>3.</td>
>>       <td>😢❌</td>
>>       <td>🤔❓</td>
>>       <td>🤔❓</td>
>>       <td>🤔❓</td>
>>       <td>😢❌</td>
>>       <td>🤔❓</td>
>>       <td>🤔❓</td>
>>       <td>😢❌</td>
>>       <td>Both data findability and accessibility will certainly take (human) effort.</td>
>>     </tr>
>>     <tr>
>>       <td>4.</td>
>>       <td>🥳✔</td>
>>       <td>🤔❓</td>
>>       <td>🤔❓</td>
>>       <td>🤔❓</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>🤔❓</td>
>>       <td>This could probably work if the university offers enough support.</td>
>>     </tr>
>>     <tr>
>>       <td>5.</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>The best solution if there is no suitable domain-specific repository.</td>
>>     </tr>
>>     <tr>
>>       <td>6.</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>The additional focus makes it even easier for you to describe your data according to the relevant standards, and for others to find it.</td>
>>     </tr>
>>   </tbody>
>> </table>
> {: .solution}
{: .challenge}

> ## Data repositories
>
> Let's examine a couple of different data repositories (maybe datasets in different repos?)
> For each of the following, [Zenodo](https://zenodo.org/), [ESGF](https://esgf.llnl.gov/), [CDS](https://cds.climate.copernicus.eu), answer the following questions:
>
> - Is this repository publicly accessible?
> - Is it free?
> - Is it proprietary?
> - Does it allow for authentication?
> - Is there any quality control for this repository?
> - Are metadata accessible, even if the data is not?
> - How long will the data be maintained?
> - Is there any backup system in place?
> - Is it easy to find data that is stored in this repository?
> - Is it easy to download data from this repository?
> - Is it easy to upload data to this repository?
>
>> ## Solution
>> <table style="width:90%">
>>   <thead>
>>     <tr>
>>       <th></th>
>>       <th>Zenodo</th>
>>       <th>ESGF</th>
>>       <th>CDS</th>
>>     </tr>
>>   </thead>
>>   <tbody>
>>     <tr>
>>       <td>1. Is this repository publicly accessible?</td>
>>       <td>🙂Most (meta)data are publicly accessible, but there are also close/restricted datasets.</td>
>>       <td>🥳Yes but account registration is required.</td>
>>       <td>🥳Yes but account registration is required.</td>
>>     </tr>
>>     <tr>
>>       <td>2. Is it free?</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>       <td>🥳✔</td>
>>     </tr>
>>     <tr>
>>       <td>3. Is it proprietary?</td>
>>       <td>🥳No. Non-proprietary format is mandatory on Zenodo.</td>
>>       <td>🥳No. Data are mostly available in NetCDF format.</td>
>>       <td>🥳No. Most datasets are in NetCDF or GRIB format.</td>
>>     </tr>
>>     <tr>
>>       <td>4. Does it allow for authentication?</td>
>>       <td>🙂A light authentication mechanism, such as a token (via OAuth 2.0 access token), is acceptable in some certain cases, e.g. high-traffic access. This authentication is acceptable as long as there is a totally open/anonymous route too.</td>
>>       <td>🙂ESGF uses the OpenID and OAuth2 authentication system. 
             Login credentials are required.
             An open source <a href="https://github.com/ESGF/esgf-auth">authentication client</a> 
             is also available.</td>
>>       <td>🙂CDS uses its <a href="https://cds.climate.copernicus.eu/api-how-to">own API and authentication key</a>. 
             Login credentials are required.
             The <a href="https://github.com/ecmwf/cdsapi">API</a> is open source.</td>
>>     </tr>
>>     <tr>
>>       <td>5. Is there any quality control for this repository?</td>
>>       <td>🙂Although not mandatory, it is highly recommended by Zenodo to include qualified references to other (meta)data. This is a quite common practice on Zenodo.</td>
>>       <td>😢Citation links and references are usually missing for many datasets.</td>
>>       <td>🙂Quite some datasets are provided with citation/reference information.</td>
>>     </tr>
>>     <tr>
>>       <td>6. Are metadata accessible, even if the data is not?</td>
>>       <td>🙂Yes for some datasets which apply this principle.</td>
>>       <td>🤔Unknown.</td>
>>       <td>🤔Unknown.</td>
>>     </tr>
>>     <tr>
>>       <td>7. How long will the data be maintained?</td>
>>       <td>🥳Lifetime of the host laboratory CERN.</td>
>>       <td>🤔Unknown.</td>
>>       <td>🤔Unknown.</td>
>>     </tr>
>>     <tr>
>>       <td>8. Is there any backup system in place?</td>
>>       <td>🥳12-hourly backup for Metadata and persistent identifiers.</td>
>>       <td>🥳Yes. Subsets of the data are replicated at Lawrence Livermore National Laboratory (LLNL) for backup.</td>
>>       <td>🥳Yes for at least all ECMWF data.</td>
>>     </tr>
>>     <tr>
>>       <td>9. Is it easy to find data that is stored in this repository?</td>
>>       <td>🥳Yes. All data are findable via DOI and well documented. There are also plenty filter available for searching.</td>
>>       <td>🤔PID is assigned per dataset. But the UI for data browsing is not friendly. Although metadata are provided, the datasets lack documentation. </td>
>>       <td>🥳Yes. All data are findable via DOI. The documentations are rich. The searching UI is quite friendly.</td>
>>     </tr>
>>     <tr>
>>       <td>10. Is it easy to download data from this repository?</td>
>>       <td>🥳Yes for data with open access.</td>
>>       <td>🥳Yes.</td>
>>       <td>🥳Yes.</td>
>>     </tr>
>>     <tr>
>>       <td>11. Is it easy to upload data to this repository?</td>
>>       <td>🥳Yes. Although one should use a Zenodo account, or an GitHub account, or an ORCID account.</td>
>>       <td>🤔In principle yes, but the procedures are complicated. To upload data to a certain project, one need a manual approval on joining that project. </td>
>>       <td>🤔In principle yes, but the procedures are complicated. One needs to contact Copernicus Climate Change Service (C3S) and fill in a confirmation form first.</td>
>>     </tr>
>>   </tbody>
>> </table>
> {: .solution}
{: .challenge}

> ## What about your data?
>
> When it comes to making data accessible, there are some easy steps
> that can by applied by any researcher to their own data. Some steps, however,
> have to be developed accross a scientific domain. Particularly, the
> establishment of domain-specific data repositories.
>
> - What is the status in your specific (sub-)domain?
> - Are there suitable repositories?
> - Are they easy to use? What are the advantages/disadvantage?
>
{: .discussion}

{% include links.md %}
