<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->


## Changes from the main branch
1. Import IFC files directly to a new table via the function
2. Buffering added at **ExtractBeforeCloseParenthesis** to improve performance
3. Extraction of Object Name and Object Type Name data

For more information, refer to <a href="https://digitalbbq.au/index.php/2024/05/16/expanding-on-ifc-metadata-extraction-in-powerbi/">Expanding on IFC Metadata Extration in PowerBI at digitalBBQ</a>

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="">
    <img src="https://github.com/shift-construction/ifc4PowerBI/assets/44708354/043504ab-7bbb-4511-be0d-6d2aa813c5ed" alt="Logo" height="80">
  </a>

<h3 align="center">IFC for PowerBI</h3>

  <p align="center">
    Pull your IFC metadata directly into PowerBI
    <br />
    <a href="https://github.com/github_username/repo_name">View Demo</a>
    ·
    <a href="https://github.com/github_username/repo_name/issues">Report Bug</a>
    ·
    <a href="https://github.com/github_username/repo_name/issues">Request Feature</a>
  </p>
</div>


</div>


<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

![image](https://github.com/shift-construction/ifc4PowerBI/assets/44708354/cb6c0fdc-5476-4363-80f2-94290f22c50d)


The goal of this function is to allow all the metadata from IFC files to be brought into PowerBI or Excel for analysis. By creating a function inside PowerQuery we have enabled teams to pull in multiple IFC models either locally or via an integration. As this is a function rather than a custom connector it also supports the cloud version of PowerBI, meaning dashboards can be automatically updated as and when new models arrive.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With

[![PowerQuery][PQuery]][PQuery-url]


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

This is one example of how to get up and running, there are plenty of different way you can use the function, or even adapt it for your own requirements.

### Prerequisites

Before you get to work you will need to have a basic understanding of the PowerBI or PowerQUery in Excel toolset and a copy of either one installed

### Installation

1. Open up the **IFC4PowerBI.pq** file in notepad or your text editor of choice
2. In PowerBI or Excel create a blank query (in PowerBI it's **Home > Get Data > Blank Query**, in Excel **Data > Get Data > From Other Sources > Blank Query**
3. Right-click the Query in the query editor (often called "Query1" in new documents) and click **Advanced Editor**
4. Paste the contents of **IFC4PowerBI.pq** into the Advanced Editor and click done
5. You now have a function for opening IFC Binary files in PowerQuery, now you need to find your binaries
6. Rename the function by right-clicking it, the name of the function will be how we reference it later, so it's best to use IFC4PowerBI
7. Find your IFC file, in Windows 11, right-click, select "Copy as path"
8. Back in PowerBI, paste the IFC path into the function text box and click "Invoke"
9. A new table will be generated named "Invoked Function"
10. Rename the table as you wish
11. Rinse and repeat for as many IFCs as your hardware can handle


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

Here are a few ideas to get you started. We have included a PowerBI .pbix file in the repository so that you can get started straight away, just find a folder with one or more IFC files

### Assess models in your CDE for compliance

By Pulling in models directly from your CDE of choice via APIs you can automatically dashboard the results, leading to quick turn around on model sutability reviews

<div align="center">
  <a href="">
    <img src="https://github.com/shift-construction/ifc4PowerBI/assets/44708354/bcc255c7-f7e5-49f4-9497-d8d00beacda5" alt="CDE" width="300">
  </a>
</div>




### Quantity Takeoff

Get your model data into Excel and use Pivot tables to understand and probe your data further

### Model Progress Metrics

By extracting the data from multiple revisions of the same model you can quantify the changes that have taken place:
- Are there more elements
- Is the metadata quality improving
- Have certain elements dissapeared


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the GPL 3.0 License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Matthew Osment - [LinkeIn](https://www.linkedin.com/in/matthew-osment/) - matthew@shift-construction.com


<p align="right">(<a href="#readme-top">back to top</a>)</p>





<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/shift-construction/ifc4PowerBI.svg?style=for-the-badge
[contributors-url]: https://github.com/shift-construction/ifc4PowerBI/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/shift-construction/ifc4PowerB.svg?style=for-the-badge
[forks-url]: https://github.com/shift-construction/ifc4PowerBI/network/members
[stars-shield]: https://img.shields.io/github/stars/shift-construction/ifc4PowerBI.svg?style=for-the-badge
[stars-url]: https://github.com/shift-construction/ifc4PowerBI/stargazers
[issues-shield]: https://img.shields.io/github/issues/shift-construction/ifc4PowerBI.svg?style=for-the-badge
[issues-url]: https://github.com/shift-construction/ifc4PowerBI/issues
[license-shield]: https://img.shields.io/github/license/shift-construction/ifc4PowerBI.svg?style=for-the-badge
[license-url]: https://github.com/shift-construction/ifc4PowerBblob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[Pquery]: https://img.shields.io/badge/PowerQuery%20M-35495E?style=for-the-badge&logoColor=1d6b40
[PQuery-url]: https://learn.microsoft.com/en-us/powerquery-m/
