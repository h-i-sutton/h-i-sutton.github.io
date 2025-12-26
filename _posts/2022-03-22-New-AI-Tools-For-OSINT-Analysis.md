---
layout: post
title: "New A.I. Tools Help OSINT Analysis Of Ukraine War"
date: "2022-03-22 23:00:00"
excerpt: <a href="https://twitter.com/covertshores" target="blank"><img align="right" src="/images/twitter.jpg"/></a><br
  clear="right"/><a href="/New-AI-Tools-For-OSINT-Analysis.html"><img align="left"
  src="/images/OSINT-AI-Ships-Count-317.jpg"/></a> Using A.I. I have been exploring
  the impact of Russia closing general access to the Kerch Straight.<br/><br/>Here
  is how.<br/>[Read More &gt;....](/New-AI-Tools-For-OSINT-Analysis.html "READ MORE")<br
  clear="left"/>
...

---
[![](/images/AmazonMyBooks.jpg)](https://www.amazon.com/s?i=stripbooks&rh=p_27%3AH+I+Sutton&s=relevancerank&text=H+I+Sutton&ref=dp_byline_sr_book_1)[![](/images/MauilTo-Icon.jpg)](mailto:hisutton.author+blog@gmail.com?subject=)[![](/images/Icon_Bluesky.jpg)](https://bsky.app/profile/covertshores.bsky.social)[![](/images/Youtube-icon.jpg)](https://www.youtube.com/channel/UCWHq3kn8PWCb66fhJD8lskQ)  

#New A.I. Tools Help OSINT Analysis Of Ukraine WarAs part of its invasion of Ukraine in late February, Russia closed general access to the Kerch Straight. This narrow waterway, with a bridge across it acting as a barrier, is the only way between the Black Sea and Sea of Azov. Several critical Ukrainian cities and ports, not least Mariupol, are in the Sea of Azov. This impacted maritime traffic, but by how much?  

Using A.I. I have been exploring the impact. Here is how.  

Open source intelligence (OSINT) is nothing new. But has been transformed by the Information Age. And the Ukraine Invasion has brought it to a much wider audience. News outlets and social media have been awash with people analyzing photos, videos and satellite imagery.   

[![](/images/OSINT-AI-Ships-Count-Before-War-450.jpg)](/images/OSINT-AI-Ships-Count-Before-War.jpg)[![](/images/OSINT-AI-Ships-Count-Before-War-Cluster-450.jpg)](/images/OSINT-AI-Ships-Count-Before-War-Cluster.jpg)  
*CLICK to enlarge. Left is raw, right is with clustering.*.  

The OSINT community has also shifted focus. Sources which were previously leveraged by relatively few analysts are increasingly exposed. Often the least dramatic and least attention grabbing sources may prove the most powerful. After all, the big picture can only be formed by connecting many sources over time.   

Then add to this artificial intelligence (AI). This is what The Intel Lab, a small consultancy, has been doing. One of the first problems to tackle is counting ships. They developed an algorithm which can spot ships in low-resolution SAR (synthetic aperture radar) satellite imagery. I have found this incredibly useful.  

![Russian military previously blocked the Kerch Strait](/images/Kerch-strait-Closed.jpg)  
*The Russian military previously blocked the Kerch Strait using a tanker in November, 2018.*  

##Technical notesThe ship detection algorithm uses Deep Learning, a branch of Machine learning. Ship detection is essentially a classification problem. But it is not a binary one; the model doesn't return a "Ship - No Ship". Instead it says "There is a ship, and here is where it is located". So it is in essence an Object Detection algorithm.  

This model was trained using Supervised Learning. Thousands of samples were manually labeled and then fed into the model for the training phase. This eventually reaching a State of the Art accuracy of over 99%.   

  
[![](/images/Book_cover_150.jpg)](http://www.amazon.com/dp/1533114870/)>>> **THE** book on Special Forces subs **[Covert Shores](http://www.amazon.com/dp/1533114870/)** **2nd Edition**. A world history of naval Special Forces, their missions and their specialist vehicles. SEALs, SBS, COMSUBIN, Sh-13, Spetsnaz, Kampfschwimmers, Commando Hubert, 4RR and many more.  
[Check it out on Amazon](http://www.amazon.com/dp/1533114870/) [![](/images/Maiale_arrow.png)](http://www.amazon.com/dp/1533114870/)  

As an optional step, a geographical clustering is added to the end. This allows aggregation of results to better show patterns. The clustering is a simple classification script based on geo-referenced feature class density. It allows the user to automatically visualize geospatial trends for further analysis.   

##Impact of War on Shipping in Sea of AzovWe focused on the Kerch Strait and Sea of Azov. Analysis of Sentinel-2 SAR imagery from before the invasion showed over 400 ships present. These were distributed between shipping lanes, anchorages and ports, with a few lose ends. After Russia restricted access through the straits this fell to just 250 ships. And many of those were at anchor south of the entrance.   

This increased after transit through the straits was resumed, but is still lower than previously.   

It is obvious how this technology could aid assessing the impact of the war. It can complement analysis of AIS (Automated Identification System) ship tracking. In the case of the Sea of Azov it very clearly captures activity which is not revealed by AIS.   

A.I. is rapidly maturing and becoming useful in OSINT. There are enhancements planned, and there are other use cases to explore.   