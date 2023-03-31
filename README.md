# anish_Ui_task

css
.body {
    box-sizing: border-box;
    width: 90%;
    margin: 20px;
    background-color: rgb(255, 255, 255);
    padding: 10px 40px;
}

.time{
    font-size: 16px;
    font-weight: bold;
}

.hour{
    font-size: 16px;
}

.general {
    float: right;
}

.date{
    font-size: 18px;
    font-weight: bold;
    color: black;

}

.call {
    font-weight: bolder;
    font-size: 1.4rem;
}

.hrclass {
    
    border-style: solid;
    border-top-width: 1px;
    border-color: grey;
    margin-top: 10px;
}

.text{
    color: grey;
    font-size: 14px;
    font-weight: 600;
}

.location{
    color: black;
    font-size: 16px;
    font-weight: bold;
    margin-top: var(--marginetopforhr);

}

.data{
    color: rgb(0 196 255);
    font-size: 16px;
}

.client-opp {
    display: flex;
    margin-top: var(--marginetopforhr);
}

.client, .opportunity{
    font-size: 16px;
    color: black;
    font-weight: bold;
}

.opp{
    margin-left: 20%;
}

.client-details,.opp-details{
    font-size: 16px;
    color: rgb(3, 45, 96);
    font-weight: 700;
}

.client-att{
    display: inline-block;
    margin-right: 10px;
    font-weight: bold;
   
}

.client-text{
    font-size: 16px;
    font-weight: bold;
}

.badge {
    background-color: gray;
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 24px;
    height: 24px;
    border-radius: 50%;
    color: black;
    font-weight: bold;
    font-size: 12px;
    line-height: 1;
    text-align: center;
    
}

/* abbr[data-original-title],
abbr[title] {
    border: 1px solid red;
    background-color: yellow;
    border-radius: 16%;
    text-decoration: underline dotted;
    cursor: help;
    border-bottom: 0;
    -webkit-text-decoration-skip-ink: none;
    text-decoration-skip-ink: none;
} */

.circle-icon {
    margin: 10px;
    display: flex;
    flex-wrap: wrap;
    align-content: space-around;
    justify-content: space-between;
    align-items: center;
    flex-direction: row;
    font-size: 10px;
}

.report {
   
    overflow: hidden;
    margin-top: 10px;
    font-size: 16px;
    padding: 10px;
    background-color: whitesmoke;
}

.icons{
    
    background-color: #2d2dff;
}

.report svg.slds-icon.slds-icon-text-default {
    height: 24px;
    width: 37px;
  }



.icons {
    color: white;
    margin-right: 10px;
}
:host(){
    --callreportcolor:blue;
    --marginetopforhr: -22px;
}
.callreport{
    color:var(--callreportcolor) ;
    color: var(--callreportcolor);
    font-weight: bolder;
}

.avtartcustom{
    margin-right: 10px;
    margin-left: 10px;
    font-size: 12px;
}



HTML


<template>
    <div class="body">
        <div>
            <span class="time">11:30AM </span>
            <span class="hour"> | 1 hr</span>
            <span class="general">General</span>
        </div>

        <div class="date">
            <span>Monday, March 30, 2023</span>
        </div>

        <div  class="call">
            Strategy Call
        </div>

        <div class="text">Meeting invite body details... Lorem ipsum dolor sit amet consectetur adipisicing elit.</div>
        <hr class="hrclass"/>

        <div>
            <div class="location">Location</div>
            <div>
                <span class="data">Outbrain Office | 11 W 19th St, New York</span>
            </div>
        </div>
        <hr class="hrclass" />

        <div class="client-opp">
            <div>
                <span class="client">Client</span><br />
                <span class="client-details">Outbrain</span>
            </div>
            <div class="opp">
                <span class="opportunity">Opportunity</span><br />
                <span class="opp-details">Equity PIPE</span>
            </div>
        </div>
        <hr class="hrclass">

        <div>
            <div class="client-att">
                <span class="client-text">Client Attendees</span>&nbsp;
                <span class="badge">5</span><br />

                <div class="circle-icon">
                    <div>
                       <span class="slds-avatar slds-avatar_circle ">
                            <abbr class="slds-avatar__initials slds-icon-standard-user" title="person name">DK</abbr>
                        </span>
                       <span class="avtartcustom">David Kostrman</span> 
                    </div>
                    <div>
                        <span class="slds-avatar slds-avatar_circle ">
                            <abbr class="slds-avatar__initials slds-icon-standard-user" title="person name">YG</abbr>
                        </span>
                        <span class="avtartcustom">Yaron Galai</span> 
                    </div>
                    <div>
                        <span class="slds-avatar slds-avatar_circle">
                            <abbr class="slds-avatar__initials slds-icon-standard-user" title="person name">JK</abbr>
                        </span>
                       <span class="avtartcustom">Jason Kivivat</span>
                    </div>
                    <div>
                        <span class="slds-avatar slds-avatar_circle">
                            <abbr class="slds-avatar__initials slds-icon-standard-user" title="person name">AW</abbr>
                        </span>
                       <span class="avtartcustom"> Arne Wolter </span>  
                    </div>   
                    
                    <div>
                        <span class="slds-avatar slds-avatar_circle">
                            <abbr class="slds-avatar__initials slds-icon-standard-user" title="person name">YC</abbr>
                        </span>
                       <span class="avtartcustom"> Yoni Cheifez</span>  
                    </div>           
                </div> &nbsp; 
            </div><br>
        </div>

        <div>
            <div class="client-att">
                <span class="client-text">Jef Attendees</span>&nbsp;
                <span class="badge">25</span><br />

                <div class="circle-icon">
                    <div>
                       <span class="slds-avatar slds-avatar_circle ">
                            <abbr class="slds-avatar__initials slds-icon-standard-user" title="person name">GK</abbr>
                        </span>
                       <span class="avtartcustom">Gaurav Kumar</span> 
                    </div>
                    <div>
                        <span class="slds-avatar slds-avatar_circle ">
                            <abbr class="slds-avatar__initials slds-icon-standard-user" title="person name">JK</abbr>
                        </span>
                        <span class="avtartcustom">Jacob Kook</span> 
                    </div>
                    <div>
                        <span class="slds-avatar slds-avatar_circle">
                            <abbr class="slds-avatar__initials slds-icon-standard-user" title="person name">AG</abbr>
                        </span>
                       <span class="avtartcustom">Adarsh Gupta </span>
                    </div>
                    <div>
                        <span class="slds-avatar slds-avatar_circle">
                            <abbr class="slds-avatar__initials slds-icon-standard-user" title="person name">RB</abbr>
                        </span>
                       <span class="avtartcustom"> Raphael Bajerano </span>  
                    </div>    
                    <div class="avtartcustom">
                       See 20 More...
                    </div>           
                </div> &nbsp; 
            </div><br>
        </div>

        <div class="report">
            <lightning-icon icon-name="utility:add" class="icons" alternative-text="Add"></lightning-icon>
            <span class="callreport">Add Call Report</span> 
        </div>

        <div class="report">
            <lightning-icon icon-name="utility:add" class="icons" alternative-text="Add"></lightning-icon>
            <span class="callreport">Add Call Report</span> 
        </div>
       
    </div>
</template>
