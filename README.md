# % Spread Between Last and SMA on components of Chain

JET2 sample application calculates the percent spread betweeen the last trade price and the user supplied number of days simple moving average (SMA) using three different API's simultaneously to show how someone can rapidly develop and deploy a useful Eikon analytic that combines streaming, historical and fundemental data with simple to use and understand TR API's.  

In SMA.html a grid is used to display, for each components of the specified Chain (put link to TR chain guide??), the following:

- [RIC](Each RIC is provided by the streaming call to the Quote object via the Chain argument)
- [Company Name](Retrieved using FID DSPLY_NAME)
- [Sector](Retrieved from call to DSS using TR.GICSSECTOR)
- [Beta](Retrieved from call to DSS using TR.WACCBeta)
- [N-Day SMA](Calculated via call to TRTH from the returned daily time series)
- [Last](Retrieved using FID CF_LAST for every streaming trade)
- [Time Stamp](Retrieved using FID CF_TIME for every streaming trade)

# Setup Sandbox and Run

- [Download and Install JET2 ZIP file]()
- [Copy JET2 files to Tomcat and start local server]()
- [Clear Eikon Cache upon any Javascript or HTML source code changes]()
- [Run SMA.html from Eikon Menubar]()

# Documentation and Video

- [See PDF file for more elaborate documentation of this sample application]()
- [See Webex video for complete soup to nuts presentation of this application]()
