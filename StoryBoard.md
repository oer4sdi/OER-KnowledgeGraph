# OER on Geospatial Web Services (in progress!).       
         	           	
## 1. Overview

In this Open Educational Resource (OER) you will learn what forms of **Geospatial Web Services** exist, how they are structured, how they can be integrated into an open source GIS (QGIS), and how they can be published via GeoServer. 

**After completing the following OER, you will know:**
* what Geospatial Web Services and OGC standards are.
* where to find and identify useful Geospatial Web Services and how they are structured
* how to integrate Web Services into QGIS and work with data from them 
* how to publish your own web services with GeoServer 

**The OER is structured as follows**.

1. overview
2. thematic background 
3. exercises and guides
4. quiz 
5. summary 

**General Information**

This tutorial is primarily intended for participants who want to spend approximately ... minutes to improve their skills in integrating data from Geospatial Web Services. At best, you should have some basic knowledge of using GIS software.

This tutorial was developed at the Institute of Geodesy at Bochum University of Applied Sciences in close cooperation with the University of Münster and the University of Bochum. The main author is Fabian Przybylak under the supervision of Prof. Dr. Carsten Keßler.

You may freely use, modify and reproduce the OER (H5P content) under the terms of the CC-BY-SA 4.0 license. Any code provided with the OER may be used under the terms of the MIT license. Please read the [full license terms](/LICENSE.md). 

The OER4SDI project was recommended by the Digital University NRW and is funded by the Ministry of Culture and Science NRW. 

## 2. thematic background

**Outline of the thematic background**. 
* Short introduction with general context and background (in a few sentences). 
* In-depth content (video format + text chordion summarizing the given information).


### 2.1 Short introduction

**What is it all about?**
The rapid development of geospatial data collection methods and techniques provides the opportunity to collect huge amounts of geospatial data. However, it also presents challenges to various data organizations and data users to manage, share, process, and analyze large volumes of geospatial data. Data organizations face the challenge of finding new solutions to manage, store, and collectively archive these vast amounts of data.

One online service to make geographic information and spatial data available over the Internet is Geospatial Web Services. These services allow users to efficiently share, search, visualize, retrieve, and analyze geographic data.

**What is the problem?**
Data dissemination systems must always deal with a heterogeneity problem. Different sources can hinder the effectiveness of sharing and managing geospatial data. Different operating systems, hardware, software, data formats, and interfaces are associated with the problem of syntactic heterogeneity. If two web services do not know each other's interfaces, they cannot exchange messages and data.

**What solution is there for this?**
For this reason, geospatial web services are typically organized according to OGC standards developed by the Open Geospatial Consortium. These standards enable the services to be interoperable and to be used across different applications and platforms.

### 2.2 In-depth content (video).

**What are Geospatial Web Services?**
Geospatial Web Services are a type of Web services that enable geospatial data and services to be provided, retrieved, and processed on the Internet. These services are typically provided by geospatial or GIS organizations, government agencies, businesses, and other entities that manage geospatial data.
![](Single_Learning_Element/Img/Slide1.png) 
**Why do you need Geospatial Web Services?**
By using Geospatial Web Services, users can access geospatial data from multiple sources, perform comprehensive analysis, and create customized applications and visualizations.

**How are GWS structured and are there prevailing standards?**
Geospatial Web Services are structured to provide geographic data and functionality over the Web. They are typically based on a client-server architecture, where the client (usually a web browser) makes a request to the server, which then returns geographic data and functionality.

Geospatial Web Services typically use one or more standardized interfaces specified by the Open Geospatial Consortium (OGC). The OGC interfaces define the format and structure of the data returned by the server, as well as the methods and parameters that can be used to query the data.
![](Single_Learning_Element/Img/Slide2.png) 
**What is the OGC?**
The OGC, or Open Geospatial Consortium, is a non-profit organization focused on developing standards for geospatial data and services. The organization was founded in 1994 and is headquartered in the USA.

The goal of the OGC is to develop and promote open standards for geospatial data and services to facilitate interoperability and exchange of geospatial data and services between different systems, applications, and organizations. OGC standards include protocols for geospatial data access (e.g., WMS, WFS, WCS), data modeling, geoprocessing, metadata, cataloging, and more.

The OGC Consortium works closely with other standards organizations and government agencies worldwide to ensure that standards for geospatial data and services are harmonized across different application domains and across different countries.

Membership in the OGC is open to organizations and individuals in the geospatial data and services industry, providing them with the opportunity to participate in standards development and benefit from collaboration with other professionals.
![](Single_Learning_Element/Img/Slide3.png) 
**What do the OGC architectural elements and the major OGC standards look like?**
The OGC Web Services architecture consists of a set of components that work together to provide the various types of geospatial web services. The major components are:

* **Service Provider:** This is the server that provides the web service and responds to requests from clients.
* **Service Requester:** This is the client that requests the web service and waits for the response from the service provider.
* **Service Registry:** This is a directory that contains information about available geospatial web services so that Service Requesters can find and use them.
* **Service Broker:** This is an intermediary that enables interoperability between different geospatial web services by translating data and requests between them.
![](Single_Learning_Element/Img/Slide4.png) 
Geospatial Web Services use open standards and protocols to facilitate the exchange of geospatial data between different systems and platforms. Key standards include: 

* Web Map Service (**WMS**). 
* Web Feature Service (**WFS**)
* Web Coverage Service (**WCS**)
* Catalog Service (**CSW**)
* Sensor Observation Service (**SOS**)

**What is the difference between the various services?**
* A Web Map Service (**WMS**) allows a client to retrieve and display static map images from a server.
* A Web Feature Service (**WFS**) allows a client to access and query vector-based geospatial data.
* A Web Coverage Service (**WCS**) provides access to and query of spatial raster data such as satellite imagery or elevation models.
* A Catalog Service (**CSW**) allows a client to search and retrieve metadata about available geospatial data and services.
* A Sensor Observation Service (**SOS**) provides access to real-time data from sensors, such as environmental sensors.
![](Single_Learning_Element/Img/Slide5.png) 
**What does a typical web request for a web map service look like?**
The Web Map Service (WMS) protocol is an interface defined by the Open Geospatial Consortium (OGC) that allows maps and geographic data to be queried and visualized over the Web. The WMS protocol defines the format and structure of the data returned from the server, as well as the methods and parameters used to query the data.

The WMS protocol uses HTTP or HTTPS as the transport protocol. A typical WMS request consists of a URL that contains various parameters that determine the content of the map. Here is an example of a WMS request and its parameters:
![](Single_Learning_Element/Img/Slide6.png) 
The server processes the request and returns the map as a response in the requested format. The map can then be displayed in the browser or in an application.

**What other requests can be made to a WMS server?**
A WMS protocol defines still other requests that can be sent from a client to a WMS server.

* **GetCapabilities:** This request allows the client to retrieve information about the available layers and capabilities of the WMS server. The response includes an XML file containing the available layers, their properties and metadata, and the supported operations and formats.
* **GetMap:** This request allows the client to retrieve a map from the server. The parameters of this request include the desired section of the map, the size and format of the map, and the desired layers and styles.
* **GetFeatureInfo:** This request allows the client to retrieve information about the features of objects at a specific point on the map. The response contains an XML file or other format containing the attributes and values of the objects.
* **DescribeLayer:** This request allows the client to retrieve information about the properties and metadata of a specific layer. The response contains an XML file or other format that contains the properties and metadata of the layer.

There are also other requests such as **GetLegendGraphic** and **GetStyles** that can be useful for specific use cases.
![](Single_Learning_Element/Img/Slide7.png) 
**What other requests can be made to a WFS server?**
A Web Feature Service (WFS) server uses different queries than a Web Map Service (WMS) server because the WFS standard focuses on accessing and querying vector-based geospatial data, while the WMS standard focuses on visualizing maps.

* **GetCapabilities:** This request allows the client to retrieve information about the available layers and features of the WFS server. The response includes an XML file containing the available layers, their properties and metadata, and the supported operations and formats.
* **DescribeFeatureType:** This request allows the client to retrieve the structure of a specific layer. The response contains an XML file that defines the properties and attributes of the layer.
* **GetFeature:** This request allows the client to retrieve vector-based geodata from one or more layers. The parameters of this request include the desired section of the data, the attributes and properties to be returned, and the filter conditions to be applied to the data.
* **Transaction:** This request allows the client to make changes to the data on the WFS server. The operations can be Insert, Update or Delete, and they are defined in an XML file that is sent to the server.

There are also other requests like **LockFeature**, **GetPropertyValue** and **GetFeatureWithLock**.
![](Single_Learning_Element/Img/Slide8.png) 
**What is GeoServer?**
GeoServer was first launched in 2001 by the Open Source Geospatial Foundation (OSGeo). The idea behind GeoServer was to create open source software that would allow users to manage and deploy geospatial data on the web.

The original version of GeoServer was developed by the Australian government agency Geoscience Australia and released as open source software. Over the years, GeoServer has been enhanced and improved by a broad community of developers who added new features and improved the performance and stability of the software.

GeoServer has enjoyed strong support from the OSGeo community since its inception. OSGeo is a non-profit organization dedicated to promoting open source geospatial software, and GeoServer is one of its most important projects. GeoServer also has an active user community and is used by many government agencies, businesses and non-profit organizations around the world.

Today, GeoServer is one of the most popular open source software solutions for geospatial data management and delivery on the web. It is known for its flexibility, scalability, and performance and is used by a growing number of developers and users worldwide.
![](Single_Learning_Element/Img/Slide9.png) 
**What are the features of GeoServer?**
GeoServer provides a platform for managing and publishing geospatial data on the web by processing data in various geospatial data formats (such as shapefiles, geotiffs, PostGIS databases) and making them available as web services (such as WMS, WFS, WCS).

GeoServer's functions include:

* **Data management:** GeoServer allows users to import and manage geospatial data from various sources. It supports various data formats, including vector and raster data, as well as databases such as PostGIS, Oracle, and MySQL.
* **Data Processing:** GeoServer can transform and filter data to provide it in various formats and projections. It can also aggregate data and create groupings to provide custom views.
* **Provision of Web Services:** GeoServer provides a wide range of web services, including Web Map Service (WMS), Web Feature Service (WFS), and Web Coverage Service (WCS). These web services allow users to easily visualize, analyze, and download geospatial data over the Internet.
* **Security:** GeoServer provides a robust security infrastructure that allows users to control access to geospatial data. It supports authentication and authorization, as well as HTTPS encryption for secure data transmission.
* **Scalability:** GeoServer can run on a variety of platforms, including desktop computers, servers, and cloud infrastructures. It is also capable of handling heavy loads and provides high availability and performance.

Overall, GeoServer is a powerful and versatile platform for managing and deploying geospatial data on the web. Which allows users to easily manage and share geospatial data, making it an important tool for geospatial data infrastructures.
![](Single_Learning_Element/Img/Slide10.png) 
## 3. exercises and guides

**Structure of the exercises and guides**. 
* Assignment 
* Video guide (screencast)

### 3.1 Exercise 1

**Required software components used in this exercise:**. 

**QGIS** is a free and open source cross-platform geographic information systems (GIS) desktop application that supports viewing, editing, printing, and analyzing geospatial data. 
(You can install **QGIS** from the [official website](https://qgis.org/de/site/forusers/download.html) and follow the instructions there.)

**Task**.

Browse for some time on the websites of the attached link collection and check which services are offered on the websites. Additionally, check in which form the services are available (WMS, WFS, etc.).

* [Geodata Catalog Germany](https://gdk.gdi-de.org/gdi-de/srv/ger/catalog.search#/home)
* [Geoportal Germany](https://www.geoportal.de/) 
* [Geodata catalog Switzerland](https://www.geocat.ch/geonetwork/srv/ger/catalog.search#/home)

Now you know some sources where you can find Geospatial Web Services. Choose a WMS and a matching WFS service and implement them in a simple QGIS project. You can also follow the attached videoguide. 

If one service does not work, try another one first. It can happen that services are no longer supported by the provider or links are out of date. 

**content of the videoguide

ssd


### 3.2 Exercise 2
**Required software components used in this exercise:**. 

**QGIS** is a free and open source cross-platform geographic information systems (GIS) desktop application that supports viewing, editing, printing, and analyzing geospatial data.

**GeoServer** is an open source server written in Java that allows users to share, process, and edit geospatial data.

**Task**

Download the provided geodata and watch the following video. Your task is to follow the screencast and host a WMS and a WFS service local on your system. Afterwards check in QGIS if you were successful by adding the services to a new QGIS project. 

If you want to go deeper into the topic, you can find more tutorials in the [official documentation](https://docs.geoserver.org/) of GeoServer. 

**content of the videoguide

ssd

## 5th quiz


## 5. summary

Hey, you did a great job! We hope you now have an idea of how to work with Geospatial Web Services like WMS and WMF Services in your GIS, and how to set up your own Web Services through Geoservers.  


**Interested in learning more?

You can find a wealth of resources on Geospatial Web Services on the Internet. Here are some recommendations: 

* [Zhao, P., & Di, L. (Eds.). (2010). Geospatial Web Services: Advances in information interoperability. IGI Global.](https://www.igi-global.com/book/geospatial-web-services/46010) 
* [Kralidis, A. T. (2007). Geospatial Web Services: The evolution of geospatial data infrastructure. In The Geospatial Web (pp. 223-228). Springer, London.](https://link.springer.com/chapter/10.1007/978-1-84628-827-2_22) 
* [van den Brink, L., Barnaghi, P., Tandy, J., Atemezing, G., Atkinson, R., Cochrane, B., ... & Janowicz, K. (2019). Best practices for publishing, querying, and using geospatial data on the web. Semantic Web, 10(1), 95-114.](https://content.iospress.com/articles/semantic-web/sw305)
* [Clabby, J. (2003). Web services explained: solutions and applications for the real world. Prentice Hall Professional.](https://books.google.be/books?hl=nl&lr=&id=AKkFqV9-_9AC&oi=fnd&pg=PR13&dq=%22fundamentals+of+web+services%22&ots=PL1iLMeHGW&sig=H9XAty66RX8LFIKAo9-VmOOEZDA#v=onepage&q=%22fundamentals%20of%20web%20services%22&f=false)
* [Link to a page or lecture describing OGC WMS in plain language](https://www.ogc.org/standards/wms/introduction) 
* [Link to a page or lecture describing OGC WFS in simple language](http://opengeospatial.github.io/e-learning/wfs/text/basic-main.html)
* [Link to Geospatial Web Services](https://gis4schools.readthedocs.io/en/latest/part2/2_1.html)


**Your feedback is welcome!

If you have identified shortcomings in this OER module or have ideas for improving the OER material, you are welcome to add entries to the issue list in the [Github repository of this OER](https://github.com/oer4sdi/Geospatial-Web-Services).
