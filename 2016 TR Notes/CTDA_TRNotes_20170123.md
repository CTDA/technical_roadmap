##CTDA Technical Roadmap Discussion
###January 23, 2017
###3:00-3:30pm EST
---

####Agenda:  
* Update on re-build of Solr index  
* Update on Storage platform  
* Update on Infrastructure discussion  
* Other business


####Notes:
* Re-building Solr index: Several participants had informed CTDA about issues with image and metadata display. Some images that had been removed were still displaying. Some information in the MODS also wasn't displaying even when configured to do so. These issues relate to the index. We were originally scheduled to re-run the index over Thanksgiving. Work was rescheduled for Christmas. We encountered issues and consulted our vendor DGI on possible fixes. One issue related directly to the jaas configuration from strict to non restrictive. We tried this in our staging environment and that worked. We just did production this past weekend. Thanks to the change, the index re-build was extremely fast and resolved the outstanding issues reported by participants and users. Thank you to all participants for halting content management activities to allow us to do this work.  
* Update on Storage: Our current storage platforms, Dell EqualLogic, will be going off warranty in the near future. Our unix administrator is being proactive to search for alternate storage platforms as the EqualLogic is being discontinued by Dell. We have several choices and our first one is to investigate Amplidata which is offered through UConn Health Center and UConn central IT. Research and testing has already begun with this new storage platform. Currently they are looking into performance testing as well as looking into speeding up performance through network enhancements. Our next sprint starting early February will continue this testing on Amplidata and make a decision whether to use Amplidata or go on and test other storage platforms.  
* Update on Infrastructure: We have a semi-distributed approach to infrastructure. Currently presentation and management sites are running on different servers. To help enhance performance, we have been investigating distributing services further to more services. Our vendor, DGI, suggested 2 possibilities and we are leaning towards one of those. In late February, we will be talking with DGI to get more specifics on that one infrastructure that we like to learn about the consequences and requirements. When we are ready to share information about any new instrcture going forward, we will discuss it at a roadmap most likely.  
* No other business
