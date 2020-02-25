# STUDIOS
### By Neema Shiramba
#### 20/2/2020

## Description
This is an app about Delani studios. It expounds on details about us and the services we offer, through this app we display a portfolio of our our past work and last but not list enable our clients contact us. 

## Behaviour Based Development
### Home page
 Add the logo using the link method show below, then typed in the content using the appropriate sizes of text as shown.

```
  <div class="back">
                    <div class="logo"><img src="IP3-master/assets/logo/logo.png"></div><br><br>
                    <H1>WELCOME</H1>
                    <h1>TO DELANI STUDIO</h1>
                    <p>AMAZING PEOPLE ARE MAKING AMAZING DESIGNS IN FUN ENVIRONMENT</p><br><br><br><br><br><br>
                    <img src="IP3-master/assets/mouse_click.png">
                </div><br><br>
```
Then add the background image using css.

### About Us and Services
This sections are simple to create and all that was needed was to place them into containers and style them using css.

### Icons
The icons were created to be able to toggle when clicked. To do this by 

```
<div class="container-fluid">
                <div class="row">
                    <div class="col-md-4 col-xs-4">
                        <div id="design"><img src="/IP3-master/assets/services_icons/design_icon.png">
                            <h6>DESIGN</h6>
                        </div>
                        <div id="content">
                            <h6><b>DESIGN</b></h6>
                            <p>
                                Our design practice offers a full range of services including brand strategy, interaction and
                                visual design and user experience testing.
                                Throughout your project, our designers create and implement visual design and workflows, solicit
                                user feedback and work with you to make sure what gets built is what is needed.
                            </p>
                        </div>
                    </div>
                    <div class="col-md-4 col-xs-4">
                        <div id="dev"><img src="IP3-master/assets/services_icons/dev_icon.png">
                            <h6>DEVELOPMENT</h6>
                        </div>
                        <div id="dev-content">
                            <h6><b>DEVELOPMENT</b></h6>
                            <p>
                                All engineers are fluent in the latest enterprise, mobile and web development technologies.
                                They collaborate with your team to write, and improve code on a daily basis, using proven
                                practices such as test-driven development and pair programming.
                            </p>
                        </div>
                    </div>
                    <div class="col-md-4 col-xs-4">
                        <div id="product"><img src="IP3-master/assets/services_icons/product_icon.png">
                            <h6>PRODUCT MANAGEMENT</h6>
                        </div>
                        <div id="prod-content">
                            <h6><b>PRODUCT MANAGEMENT</b></h6>
                            <p>
                                Planning and development is iterative. Because we are constantly coding and testing, the
                                products we build are always ready to go live.
                                This iterative process allows for changes as business requirements evolve.
                            </p>
                        </div>
                    </div>
                </div>
```
then add the following Javascript to make it function as wanted, using the classes that were assigned above.

```
  $("div#design").click(function() {
      $("div#content").toggle();
      $("div#design").toggle();
    });
    $("div#content").click(function() {
      $("div#content").toggle();
      $("div#design").toggle();
    });
    $("div#dev").click(function() {
      $("div#dev-content").toggle();
      $("div#dev").toggle();
    });
    $("div#dev-content").click(function() {
      $("div#dev-content").toggle();
      $("div#dev").toggle();
    });
    $("div#product").click(function() {
      $("div#prod-content").toggle();
      $("div#product").toggle();
    });
    $("div#prod-content").click(function() {
      $("div#prod-content").toggle();
     $("div#product").toggle();
    });
```

### Portfolio
In the portfolio section they where eight different portfolios.first thing to do is place them in the the following classes;
```
<div class="container">
                    <div class="row">
```
Then place each portfolio inside it's own column class so that we will be able to edit each portfolio individually.

```
<div id="photo1">
                                <img src="IP3-master/assets/portfolio/work4.jpg" class="img-responsive" width="100%">
                            </div>
                            <div id="text1" class="fade"><p>Black theme</p></div>
                        </div>
```
To add the hover effect when the mouse is ontop of on each portfolio, we add the following javascript.

```
 $("#col-1").hover(function() {
      $("#text1").fadeTo("slow",1);
      $("#photo1").fadeTo("slow",0.4);
      },function() {
        $("#text1").fadeTo("slow",0);
        $("#photo1").fadeTo("slow",1);
      });
```

### The Footer
The final part of the page is to name and the year it was published. 
```
 <div class="end">
                <p>DELANI STUDIO</p>
                <P>2020</P>
            </div>
```
### Known Bugs
If you find any issues in the code feel free to [click here](https://neema-bmb.github.io/Delani/)

### Technologies Used
I used:
HTML, Bootstrap, CSS, jQuery & Javascript.

### Contact me on: neemashiramba@gmail.com
I encourage anyone who has any contribution to make to this code to improve it do so. 
Live link:https://neema-bmb.github.io/Delani/


### License
App is licenced by [MIT.licensing](LICENCE.txt)
