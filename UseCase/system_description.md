Project Brief: Travel Reservation System (Focus on car rental reservation) Course: ITCS371 
Good morning, guys. I will describe the project topics for your group. I will act as the Business Analyst for this project.
I have talked to our customer, and we have to develop the software for them. Our customer wants to join the travel business, specifically in terms of a booking and reservation system. You can think of Booking.com or Agoda. They want to compete with Booking.com and Agoda, which is quite a "red ocean" in the travel business where everyone has their own booking system. However, we still have to develop this software for them.
Here is a summary of the requirements after my discussion with the customer.
1. System Overview The system is called "Travel Naja." It covers three main reservation platforms:
Flight Ticket Reservations
Car Rental Reservations
Room Reservations
These are the three basic components: Flight, Car, and Hotel. Additionally, they want a "Plus One" feature: Local Guide Tour Booking. Their goal is to merge every existing booking service into their platform.
2. User Roles
General Users (Front-end): These are general people visiting the website. They can view promotions and public content. To make a reservation, they must fill in their profile and payment details to become a member. Once registered, they can use the reservation features.
Back-end Staff: The platform acts as a middleman. We don't own the inventory (rooms/cars). The back-end staff acts primarily as report generators for the executives—tracking data like how many users booked flights this month or what the most popular destinations are for strategic planning.
3. External Agencies (APIs) Our platform must communicate with four key parties. For the first three, we need to connect with their Agencies/APIs:
Flight Ticket Agency: You must write software to communicate with their API to get flight lists and pass reservations to them.
Car Rental Agency: Handles car types, availability, dates, and locations. Our platform simply lists what is available based on their data.
Hotel Reservation Agency: Similar to the others, we fetch room availability from their API and display it on our webpage.
4. Local Guide Management (Internal) Unlike the other three, we cannot find an agency to handle Local Guides, so our platform must manage this internally.
Process: Local guides cannot input data directly. They must submit a request form specifying their talent, expertise, tour style, and program.
Validation: Back-end staff will review these requests to guarantee quality. Once approved by staff, the tour appears on the website for users to book.
Capacity: The system must enforce a maximum capacity (e.g., if a guide can only take 10-20 people).
5. Payment System Since this is a new platform, we will start with Credit Card payments only. You must write the platform to communicate with the bank's credit card gateway and ensure the system can successfully deduct money.
6. Platform Requirements
Web: A website is required for desktop browsing.
Mobile: Native applications are required for both iOS and Android.
Scalability: The system must handle thousands of transactions per second. They anticipate over 10,000 customers per month. This includes both incoming traffic (users) and outgoing traffic (API calls).
7. Reporting & Data You can explore data requirements from Agoda or Booking.com as a reference. The system needs a report management system for strategy planning, covering at least reservations from all agencies and statistics for local guide tours.
8. Security We handle global transactions and sensitive data flow. The client requires maximum encryption techniques for secure communication between our platform and the agencies. Note that high-level encryption requires high computing power, which may conflict with the scalability requirement. This will be a tricky part of your architecture design.
9. Advanced Search & Personalization This is a crucial part. We need a unified search interface where a customer specifies a destination and schedule, and the system provides a list of available flights, cars, and rooms.
Personalization: We need comprehensive customer profiles (e.g., preferred accommodation style like hotel vs. apartment, number of travelers to recommend SUV vs. sedan, or ticket class like business class vs. leisure).
Recommendation: The system should intelligently recommend options based on these inputs.
10. Development Priority The highest priority is Flight Ticket Reservations and Payment. These must be implemented and delivered first. Room and Car reservations can come later.
Enjoy the first phase of the project. If you have questions, please text me. Good luck!






(Transcribed by TurboScribe.ai. Go Unlimited to remove this message.)

Okay, good morning guys So I will describe your project topics For your group. Okay. Let me see my note Okay, so first of all, I would like to say that I will be your business analyst Business analyst for your group. 

So I have talked to our customer and then we have to develop the software Fredim, okay. Okay our customer want to join the business, the traveling business, but in the term of booking reservation system. You can think of booking.com, Agoda. 

They want to compete with booking.com and Akoda. Okay, which is quite a red ocean of the traveling business where everyone have their own booking system Okay, but yeah, anyway, we have to develop a software for them Okay, let me Summary, let me give you a summary of our requirements after I have talked to the customer Okay, what they want for their system. Okay, let's get started. 

Okay, first of all this system is called “Travel naja Travel naja system.” So the system cover three main reservations Platform first one and flight ticket reservations second one car rental Reservations and the third one is room Reservations that is three main basic reservations component for this system flight booking Car rental and Hotel reservations. Okay, and then they want to have a plus one Business Plus one feature. 

This feature is for booking a local guide tour. They want to merge Every existing booking in this world into their platform and then they we have to serve them well Okay, let's start with some more detail. Okay, let's start with The users for this system First one They are the general users so it's like general people come to see the website, okay come to see the website and then They they can see the promotions. 

They can see the Publishers content public content and then they have to To fill in their profile to fill in their Payment details to become a membership. Okay after they get enrolled to a To be a member they can use those Reservation system and then the booking features. Okay from user from general user Make a register and then it's become a memberships And That that is the first group the front-end group and then the back-end group for the back-end group the back-end user so actually they want to be a this platform will act as a middleman for for the reservations, so we actually don't have to maintain all the All the booking available all the room available by by ourself we The the back-end staff will act like a report generator for the executive That that is what they they actually Respond for like how many user booking the flight during this month. 

What is the Most Pretentious place that they want to go something like that in terms of the Strategy planning later. Okay, but the crucial part is that our platform must be communicate with the agency Okay, so we got four agencies Involved with our system first one flight ticket agency. Okay, so you have to write a software to communicate with the API to get the list of flight ticket and Pass the the reservations to the flight ticket Agency, that is the first one second one car rental agency. 

That is The agency that handle our car rental reservations. Okay times type of cars days Locations Destinations those is more about car rental. Okay, our car rental agency will handle this our website Okay, just our platform just list what car available Okay, and then those data those available car rental data come from The agency, okay, and then the third agency It is the hotel reservation agencies as you can see it is the same later and Just handle all the room available all the place Hotel valuable. 

No, we just get the data from the API And then what we just do is just display on our web page. So we have three external party Flight ticket agency Hotel reservation agency and then car rental agencies, okay but for local guide we have to maintain it by ourself because we can't our customers cannot find an agency to handle this local guide management So our platform must handle this part by our own. Let's say The back-end staff must be able to Input the list of local guide available. 

We don't allow the local guide to input the system to To to input the information to our system directly they have to Okay for the local guide. Okay, this is another user of our system The local guide must submit a request form to the website and then specify their Talent their expert area their style of the Tour the program of the tour so and so I think you you can imagine about what? Requirements what there are requirements that we require from them Okay after they send the request to To our system and the back-end staff will see those requests to to to be a local guide and then they can Approve whether this one is Guarantee the quality of the tour so our platform do not handle the the checking the Validation of those local tour list the back-end staff will do by themselves What we just do for our platform is that we provide information for them. We provide information that The local guide to submit the request form and then once the the the back-end staff validate The tour validate the local tour the local guide tour they can just approve and Approve to our system and then the the that Particular local guide tour will appear on the website allow all the user and member to To reserve for that tour But what we have to maintain is that we have to maintain the maximum capacity of the tour like if they Provide only 10 or 20 people. 

So our system must maintain that capacity. Okay Okay, that that is the major Information of our system. Let's talk a little bit in detail for the payment Since this is new platform, they don't have much choice for the payment. 

So right now They asked us to provide a credit card payment for for their customer so every payment will make to a credit card, so we have to find a way to write our platform and to Communicate with bank credit card system. Okay, we have to make sure that our system can can Like deduct their money Through a credit card system. Okay Let me check what else that we have Okay, the system must be available like a native Applications for both iOS and Android for the desktop they have To they require to have a website. 

Okay, let's say we have to provide them a website for Just desktop browsing. Okay, but if that user Access the system from their mobile phone either iOS or Android system We need to provide them as a native app. Okay, and Then There are some scalability requirements there. 

So they require to handle Thousands transactions per seconds. They imagine like they will have more than 10,000 customer per month Okay, that is They require us to handle thousand transactions both internal transaction and external transactions both incoming incoming from user and then outgoing like from our platform to those agencies, okay, and then What else for for the domain Explorations you can explore the data requirements from a coda booking.com that will be The similar case so you can get some data requirements from there. Okay Next would be about the report management system so as as I mentioned This system they also emphasize on the strategy planning, so I'm not sure whether how How they want the report but our system must provide all kind of report at least the reservation through all agencies and the statistical report of the local guide tour Okay Another one requirements is more about the security because as you can see we have different type of Sorry, we have different type of incoming and outgoing flow of the data From users which is they're supposed to handle Transactions from all over the world okay, and We have outgoing flow which is from us to those agencies those API they requires to have a maximum encryption techniques Okay, which is I don't know. 

What is it, but you have to Take care of this there one Fancy and advanced encryption techniques or Secure communications from our platform to those agencies Okay that's also a concern about a scalability and maintainability because those advanced encryption techniques would require a high computing power Which is quite conflict with the requirements of scalability this would be a trick a tricky part for your design in term of Architecture design. Okay, and then let let me check what what we have here so far This the system must provide an advanced Searching Okay, this is a crucial part of our system because we integrate all three agencies together flight ticket car and room reservations Our major part is that we have to provide a nice interface a nice searching system for them for their customer like That they they mentioned something like okay, let's customer specify just destination and schedule and our platform can provide The list of available flight ticket the list of available car reservations and the list of available room for different kind of Hotels and in term of doing that We have to get a quite comprehensive customer profile for example like style they want to live in hotel motel or flatmate Okay, and then a number of people that they travel with in order to recommend the the car system not not the car system the car reservation like a big car SUV or just sedan and then the Height of ticket of flight ticket that's suitable for their For their for their trips for example a business seat for those who are Leisure trips something like that. Okay, so you need to think of those Experientially the user requires to input some particular information and then the our system can recommend different kind different types of Those flight ticket available car available and room available that that is what they they focus and then they The expectations of our system, okay But in term of development planning in term of software release The most priority like the the highest Priority is more about flight ticket reservations and payment Okay, they need to We need to quickly provide them the the flight ticket system first the loom reservation and car reservations can come later after the flight ticket Pipeline is implemented and delivered to their customers Okay That is Most of the details that I can deliver for you right now After you see this video clip and then if you have any questions, please text me and then I will get a Qualifications for you guys. 

Okay. Enjoy your first phase of the project for traveling system Okay. Bye. 

Bye. Hope you Do a good job. See you again later

(Transcribed by TurboScribe.ai. Go Unlimited to remove this message.)


