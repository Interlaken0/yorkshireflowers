<img width="1097" height="561" alt="image" src="https://github.com/user-attachments/assets/07462644-98fc-4a3d-912b-50d0aaee7b0b" />

<img width="1782" height="475" alt="image" src="https://github.com/user-attachments/assets/896a4af0-1f82-48f2-bb3c-24c94d9e5289" />

Situation
My project started with a simple static front-end repository for a small local business named "The Yorkshire Floral Co." While the HTML/CSS provided a beautiful User Interface (UI), there was no back-end functionality at all to receive or forward the customer contact form.

Task
For my MVP project, the main goal was to get the contact form working without developing or maintaining a custom back-end server. I had to create a serverless automated data pipeline that would be able to capture, route, and store user-submitted data from the time they clicked submit until the final destination.

Action
I completed the following tasks to link together static code and dynamic functionality:

Deployed the forked repository to Netlify.

Configured the raw HTML form attributes, specifically adding Netlify's flag and name attributes so that their bot could intercept and forward the submission data.

Used Zapier to serve as the central hub for handling the flow of data. I created a webhook trigger for when new Netlify form submissions were received.

Mapped out the dynamic payload to perform two separate tasks after receipt. First task = dynamically format and send the submission details via Zapier to a designated Gmail inbox. Second task = create a new log entry in a Google Sheet database.

Results
With success, I now have a fully live, production-ready version of the website. Every time a customer clicks "Get in Touch!", the serverless pipeline will automatically and instantaneously send their inquiry to both an email inbox where someone can respond immediately, and also add them to a spreadsheet for future reference for lead tracking.

Impact
The completion of my MVP has been amazing and allowed me to experience firsthand modern automation. I gained knowledge about deploying to the cloud and how Continuous Integration works in real-world environments. More importantly than anything else though, it showed me just how powerful serverless architecture is and how easily it is possible to connect different APIs and pass around complex data streams through multiple interfaces without having to develop or maintain a full-featured back-end server.
