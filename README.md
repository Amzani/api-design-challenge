# API Design Workshop


## Requirements

- Unix/Linux Shell
- [Dredd](http://dredd.readthedocs.io/en/latest/)
- [Postman](https://www.getpostman.com/)
- draw.io
- Read [Adidas API Guidelines](https://adidas-group.gitbooks.io/api-guidelines/content/)

## Design

You have as business goal to build a killer video sharing app! that must be cross-devices (Desktop, Mobile, AppTV...)

You've decided wisly to think [API First](https://adidas-group.gitbooks.io/api-guidelines/content/core-principles/api-first.html) and [API Design First](https://adidas-group.gitbooks.io/api-guidelines/content/core-principles/design-maturity.html).


## User stories

- As a user, I want to upload my videos.
- As a user, I want to retreive my uploaded videos.
- As a user, I want to update my videos metadata (title, description).
- As a user, I want to share my videos to other users.
- As a user, I want to play one specific video.
- As a user, I want to delete my videos.

## Step1. Let's create a state machine diagram

Task: In this step we draw out a state diagrams for the proposed API. Each box in the diagram represents a possible representation. You can use arrows to indicate transitions from one box to the next.

You can use [draw.io](draw.io)

This state machine diagram will help you to identify the main ressources and their relations.


## Step2. Let's describe what actions our API affords

List all the API affordances


## Step3. Formalize the design in the [Open API Specification](http://swagger.io/specification/)

Task: Write an open api specification


> The OAS file can be edited in whatever tool you like *BUT NOT GENERATED FROM YOUR CODE*, the most important thing is that the aprouved one (the contract) *MUST* be in Apiary.



## Step4. Verify the design using Apiary Documentation and Apiary Mock Service

Task: Try the Apiary mock service

## Step5. Review the API Design


At this stage you:

- Ask feedback from your API users by sending to them the documentation link.
- Ask feedback from your product owner
- Ask feedback from the API Evangelists (if needed :))

If your API looks like this remote control then your design is affordant and consistent.

![Grandma Remote control](https://raw.githubusercontent.com/Amzani/api-lifecycle-tutorial/master/img/remote.webp)



## (Optional) Develop the API

### Dev workflow

1. Check out the VCS repository with the OAS file
2. Set up the Dredd [API testing tool](https://github.com/apiaryio/dredd) locally
3. Configure dredd for your project
4. Run dredd 
5. Implement the API (Keep running the Dredd locally to see the progress.)
6. Set up a CI/CD pipeline to execute the Dredd tests automatically


### Test with postman

1. Import the OAS file into postman
2. Run the demo video api app (npm start)
2. Test the API with postman



## Some example of good designed APIs

Sample APIs following the guidelines are available at [adidas-group GitHub](https://github.com/adidas-group). The samples include the following:


### [Simple API](https://github.com/adidas-group/demo-simple-api)
Very simple API including implementation, testing, and full CI/CD lifecycle.

### [Approval API](https://github.com/adidas-group/demo-approval-api)
Real-world API with state transition, API key client app authentication, exposed via API management.

### [Orders API](https://github.com/adidas-group/demo-orders-api)
Sample API used as the template for newly created projects at Apiary.

### [Inventory API](https://eainventoryapi.docs.apiary.io/)
Real-world Adidas Inventory API (WIP)

### [Appointment Service](https://github.com/adidas-group/demo-appointment-service)
Demo API, including implementation and testing used during training.

### [Complex Search Parameters](https://github.com/adidas-group/demo-complex-search)
Sample API showcasing description of complex query parameter rules.

### [CPM] Asset Trafficker https://assetmanager4.docs.apiary.io/



## Some example of bad designed APIs

### [[Sales and Distribution] Returns Confirmation API](https://returnsconfirmation.docs.apiary.io/)
Missing description
Missing examples
Missing HAL
Exposing internal model
Missing support contact

### [ATP Notification Service](https://atpnotificationservice.docs.apiary.io/)
Usage of acronyms, what's ATP ?
Missing description / context
Missing HAL
Missing support contact




