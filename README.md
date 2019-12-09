Description of the project:-

A tenant-owner application where owners publish ads for their house/room rent. A tenant can view all the houses without logging in but to contact the owner they have to sign-in. Tenant can request for the house and owner can view all the requests for renting the house in their dashboard. The owner can chat with the applied tenant and accept whomever he wants.
Both tenant and user can login and update their profile. The owner can pay their rent directly throught the platform (still not added all the features for it, might be using the stripe API at some point). The tenant can file a complain against any occurance and the message this will be pushed to the owner immediately.
Owner can also have managers under him to maintain his/her house. The owner and tenant can directly chat, they can see who is currently active and there are notitifications for the ofline messages when one logins to the platform.

Technologies Used:-

The project is build using Laravel. The framework of the MVC is well maintained. 
MySql is used as database, ajax and javaScript for building the chatting system.
Eloquent is used for cleating tables and querrieng values from DB. At some places for complex data fetching, raw querry is used which is the function of eloquent. You will get some good understanding of db querries related with inner-join, searche insert and update, all with the eloquent.
Bootstrap, HTML, CSS and the blade templeting is used for front-end
The entire website is responsive so that it can be seamlessly used on mobile device with out breaking any visual representation 


Steps to run the project:-

1) Install Xampp, composer and npm. If you already have then then it's great.
2) Copy the project and put it to your htdocs folder.
3) Go to your VS code terminal (I prefer using VS code) and if you are not having it then you can simply open any bash            terminal and run the following command:- 
   "composer update" it will  then it will update all the packages in your local copy.
4) Go to your xampp folder then apache->conf->extra and open the httpd-vhosts.conf file. At the bottom add the following          lines:-
            <VirtualHost *:80>
            DocumentRoot "c:/xampp/htdocs/RentRaction/public"
            ServerName rentraction.test
            <Directory "c:/xampp/htdocs/RentRaction">
            </Directory>
            </VirtualHost>
Make sure to change the directoryName and the DpccumentRoot  as your xampp's drive where you have installed it.

5) Now go to "C:\Windows\System32\Drivers\etc\" and open the "hosts" file in your notepad/nodepad++, make sure you are in       administration mode. At the bottom of the file add "172.0.0.1  rentraction.test" and save it.
6) Close the Xampp and start the Apache and MySql again. 

You should be good to start the project. Go to the browser and type rentraction.test
