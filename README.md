Introduction
=============

This software is open source, works as a WAF module in Nginx web server, and it provides 
a lightweight and restful framework for us to look into the content of requests from clients.

It can defend amount of attacks, such as COMMAND/XSS/SQL/HEADER injection,
upload file attack, slow HTTP DOS, hash consistency attack, etc.
    
Also, it provides an effective way to monitor the Nginx web server in real time,
supports IP whitelists and blacklists, and works with log system for further study.

Features
=============

1. Flexible Rule Engine:

	A flexible rule engine sits in the heart of YY SEC WAF.

2. Effecient Regex Engine:

	I am please to choose PCRE as regex engine for YY SEC WAF.

3. Real-Time Monitoring and Attack Detection:

	YY SEC WAF can monitor the HTTP traffic in real time in order to detect attacks. 
	In this case YY SEC WAF operates as a web intrusion detection tool, allowing you
	to react to suspicious events that take place at your web systems.

4. Network-Based Deployment:

	YY SEC WAF works equally well when deployed as part of a reverse proxy server,
	and many of our customers choose to do so. In this scenario, one installation 
	of YY SEC WAF can protect any number or type of back-end web servers.

5. Embedded Deployment:

	YY SEC WAF is an embeddable web application firewall, which means it can be 
	deployed as part of your existing web server infrastructure (Nginx).

Install
=============

To make things simpler, i just write a simple Makefile to compile source file.
You may cann't use it directly, just feel free to improve it for yourselves.

    Dependencies:
    apt-get install libpcre3 libpcre3-dev
    apt-get install zlib1g zlib1g-dev
    apt-get install openssl openssl-dev

    make

Test
=============

    prove -r t/

    run the test case.

About
=============

	nginx-http-yy-sec-waf-module

Copyright (C) YY, Inc.
