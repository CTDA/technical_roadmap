##CTDA Technical Roadmap Discussion
###August 22, 2016
###3:00-3:30pm EST
---
####Notes:
* The new tools are being tested: GIS tool and ordered newspaper issue batch. The GIS tool will allow users to download the OBJ datastream for any object where the type of resource in the MODS is cartographic. The ordered newspaper issue batch allows users to zip multiple issues and an issues' pages without having to put each page in a separate folder. Both of these tools will be rolled out at the end of the next maintenance sprint.
* DGI has completed a patch to the binary object content model that will allow us to run batch ingests such as the one used for electronic regulations from sites where Islandora is at head alleviating the need to run this on sites with outdated software.
* MODS to DC xslt: We noticed that our mapping was inconsistent. We found that during an update that the custom xslt had been reverted to the default. We have updated that default with our custom and have now made a note to ensure that the mods to dc transformation remains our custom one for any updates.
* We now have a public dashboard that monitors loading times for our sites using the software called PRTG. For our annual review, we will be looking at average load times and up times for each site.
* Some users have been ingesting corrupted tiffs and pdfs. This is affecting Djatoka in particular and shutting it down. We will have to keep an eye out on this. A message has been shared with participants' to ensure that their content isn't corrupted.
* Workshop on Open Refine and MODS: On Sept. 26, 2016, there will be a full day workshop covering Open Refine, xml, MODS and if there's time xsl. This workshop will be held at the Avon Free Public Library in their computer lab.
* Batch report module: This should remain disabled for the time being.
* Report on DGI's webinar on GSearcher and Tripplestore adapter:  
On July 27, 2016, DGI presented their GSearcher and Tripplestore options for clients. They explained the limitations of Mulgara which are an inability to cluster or balance the load, incomplete sparql documentation, inability to scale, and inactive project. GSearcher is meant to alleviate some of the pressure on Fedora's gsearch. The Tripplestore works as an alternative to Mulgara and works best by splitting functions onto multiple servers. The Tripplestore implements among other things Blazegraph which is being considered for Fedora 4. The good news is that several institutions have implemented successfully both GSearcher and Tripplestore. U of T has a patch that helps with those institutions that have multiple namespaces. DGI's tests have been with a repo of 1 million and would like to see how this scales up to a repo of 60 million objects. There are instructions on how to implement this on GitHub. For those who are familiar with the process, it takes approximately 2-3 days.

* Discussion on rhel7, mariaDB, and infrastructure:  
rhel7 is a big change from rhel6. Users won't notice this change as their interactions are at the application level. However, at the systems level there are differences that our administrator is currently researching and testing. In time, we will have to migrate everything to rhel7 as rhel6 will no longer be supported. MariaDB is the replacement for MySQL in rhel7. The current version of mariaDB is 10. To go to this, we'll need to go to MySQL 5.5 and then mariaDB 10. This has already been done successfully by many other places and our admin expects this transition to be fairly straightforward. The positives with going to rhel7 and especially mariaDB is that mariaDB comes with a host of database engines to select from and provides better performance especially compared to the MySQL 5.0 which we currently run. It would be interesting to test rhel7 and mariaDB with the gsearcher and tripplestore options. This leads us to think about a different infrastructure than what we current have. We are somewhat distributed. It would be interesting to further distribute tasks. Over the next couple of months, we'll be discussing those options. One thing we need to think of are functional goals and use cases to help us think about an infrastructure that will enhance not just performance but also user experience.