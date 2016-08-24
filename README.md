# Responsive Images: Project Part 1

## Setting up IIS Server

1. First you must turn on IIS: Start>Control Panel>Programs>Turn Windows features on or off. The Windows Features box will appear. It may take a while for it to load. Scroll down and find Internet Information Services and ensure the box is clicked. Underneath that is Internet Information Services Hostable Web Core. Click that box as well.
2. Second you must open the Internet Information Services (IIS) Manager and configure IIS. Click the Start button and type IIS in the search bar. Click on Internet Information Services (IIS) Manager to open. In the left Connections pane click the little arrowhead to open the tree and right click on the Sites folder. Click Add Web Site. Give the site a name, and add the path to the folder where your website is located. Go to the IP address and click the drop down. Find the IP address (ex. 192.168.0.92). (write this down somewhere. I put it as comments in my html and css files). Pick a port. I don't recommend using port 80 but any other should do. I used 90. Click ok.
3. Third, set read permissions on the website folder. Right-click on the folder your website is kept on and click on properties. Go to the security tab and scroll through Group or user names and look for the following:
  ``IUSR and IIS_IUSRS``
4. If they are there, be sure that "read & execute" and "read" are checked. If they are there and not checked click on on of them and then click edit. check the box for read & execute and read. Click apply then click ok.
If they are not there then click edit and then Add. This brings up the Select Users or Groups box.
5. Click the Advanced Button and then the Find Now button. Scroll down until you find IIS_IUSRS. Click on it and press OK 2 times. Click apply.
6. Repeat for IUSR

__Note: Don't forget to change security/permissions for IIS* files/folders__

## Running Server
1. To bring up website on local host

2. Open Chrome and type in the IP address and port like this:
``192.168.0.142:90``(or whatever your port number is)

####I hope this helps. Good luck####


## Video for Windows Setup:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=A_0SqnOPSng
" target="_blank"><img src="http://img.youtube.com/vi/A_0SqnOPSng/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>


##Project Part 1 Tests
1. ``<img>s have max-widths of 100%``
2. ``<article>s are reasonably wide (600-1200px)``
3. ``Page bytes are under 1.5MB (refresh to update)``

##Project Part 2 Tests
1. ``smiley_face.png is gone``
2. ``<meta> has charset set to utf-8``
3. ``Smiley face is unicode``
4. ``Flourish is gone``
5. ``A Twitter font icon is on the page``
6. ``A Digg font icon is on the page``
7. ``A Facebook font icon is on the page``
8. ``A Google+ font icon is on the page``

##Project Part 3 Tests
1. ``There are 8 <picture>s on the page``
2. ``There are 2 <sources>s per <picture>``
3. ``There is 1 <img> per <picture>``
4. ``<img> is last child of all <picture>s``
5. ``Every <img> has an alt attribute``
