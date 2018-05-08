We worked with the College IT department to develop software that will extend the functionality of Netbox an open source inventory management solution. Netbox is used to rack and manage hardware in a network. Our group was tasked with creating a version which added a multiple field search and could better handle items not connected to the network. To do this we made a wrapper that presents itself as a sidebar over the existing Netbox UI. This sidebar contains all the search fields as well as buttons to reach the homepage and add page.

Netbox is mostly written in Python with some html, css, and javascript, but since what we created is a wrapper our code is contained within a single html file named FrontEndCSS.html. In this file we use CSS for formatting and Javascript to access Netbox's API. When our program starts it displays the Netbox homepage and our search bar. Our search function works by calling get from the Netbox restful API. The get function finds corresponding devices in the database. These devices are returned as a JSON object which we use to generate our search results.

One thing that we wish we could have gotten to that we didn't is creating a better report system. Ideally we would have also implemented a system to track when items move locations, so that we could generate reports that include a history of location changes. 

One of our groups major contributions to the NetBox experience is the introduction of searching by mulitple fields. This allows users to effectively narrow search results with fewer queries with a more intuitive interface.

Project Dependencies:
Functioning NetBox installation
Modern Browser
