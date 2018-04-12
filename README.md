This git shows rendering tableau vizualization on salesforce. 

Step 1: Create a tableau vizualization and publish to the server

Step 2: Create a vf page and add the link to the vizulaization

There are 2 ways to do this 

1) Purely through <apex:iframe> 
2) Use tableau's javascript API

I found that the rendering is better through JS API hence used this approach. If you prefer to use iframe it would as simple as using

<apex:iframe src="#defineyourulhere" />

Either way set cache="true" on your VF page.  Read more about caching behavior and how to control cache time from here :
https://help.salesforce.com/articleView?id=sites_caching.htm&type=5
