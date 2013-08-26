#Scroller/UI Tab Scroller
This plugin can add a horizontal scroll ui in the form of buttons, one to scroll left and the other to scroll right, to any "unordered" list,this can also be implemented for jquery ui tabs and more.(Since Jquery UI 1.10.3)

## Installation

To install copy the *javascripts* and *stylesheets* directories into your project and add the following snippet to the header:

    <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.0.2/jquery.min.js" type="text/javascript"></script>
    <script src="js/jquery.scroller.js" type="text/javascript"></script>

See examples to decide on a stylesheet
    
***
###Options

These are the defaults settings for Scroller:

    proportion:0.93,        //The size of slideable area percentage or decimal
    space:'auto',           //Space between list elements 
    selection:'li[aria-selected=true]',
    html:'',                 //Button Html example {buttonLeft:'left',buttonRight:'right'}
    bspace:0,                //Space between button and list(setter)
    background:''           //For UI Implementation {position:'',css:{background:'red'}}
    
***
###Methods

    reset       //Reposition list left to zero
    getLast     //Get last item still in view
    getFirst    //Get first item still in view
    isOver      //Boolean is there an item over viewport
    isUnder     //Boolean is there an item under viewport
    refit       //Place selection item in view
    resize      //Resize list if window size increases
    forceResize
    update      //Update list size according to parent container
    repositionButton    //Realign buttons with list
    
    

All of these methods are chainable except for isOver and isUnder

$('#test').scroller().scroller('refit')

Examples include general setup and setup for Jquery UI tabs