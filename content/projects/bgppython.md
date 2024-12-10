+++
title = "BGP and Internet Access in the Circumpolar North"
date = "2023-12-09T22:14:54-09:00"
#dateFormat = "2006-01-02" # This value can be configured for per-post date formatting
author = ""
authorTwitter = "" #do not include @
cover = ""
keywords = ["", ""]
description = ""
showFullContent = false
readingTime = false
hideComments = false
+++

# Understanding the Internet Backbone in the Circumpolar North

I was the lead author on a paper addressing internet access in the circumpolar north that addressed BGP and ASes. Border Gateway Protocol (BGP) is the protocol that governs communcation between Networks (also called Autonomous Systems) or ASes. These networks are administered by Internet Service Providers or ISPs. I presented the paper at INFOCOM 2024 in Kingston, ON, Canada. I also presented a posterboard version of the paper at the Murdock Undergraduate Science Conference 2024 in Vancouver, WA.

Read it here: [CCCE_24_DmDuo.pdf](/projects/CCECE_24_DmDuo.pdf)

# BGP Python AS Lookup

The development of BGP python AS lookup was inspired by a repository found on Cisco Developer (pyjoeypy06). I thought that the code was interesting and learned of the API it was using to pull the BGP data from the internet.  The API seemed underutilized so I set out to make more use of it.  The app works by appending the entered ASN to a link to the api, which then responds with JSON data.  It then parses through the JSON data for the specific information each section of information may need for the given AS.  The information is stored in object variables so the app can store more than one AS’s data.   It uses string concatenation to display the result in plaintext format.The project was built in Python and the UI was built using TKinter (a built in python graphics library). 

![app1](/bgp/moro_app_1.png)
![app2](/bgp/moro_app_2.png)

https://github.com/UnderYourSpell/BGP_python_AS_Lookup