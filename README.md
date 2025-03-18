# Overview

This repository contains the code that is used to extract the addresses in an Amazon Flex itinerary and optimizes it using Google API.

# Background

## Amazon Flex

Amazon Flex is Amazon’s gig-economy delivery program that enables independent contractors to deliver packages using their own vehicles. Drivers use a dedicated mobile app to sign up for delivery blocks, pick up packages from local hubs or partner locations, and then deliver them directly to customers. This flexible work model allows drivers to choose their own hours, making it a popular side hustle or full-time opportunity in some regions.

## Pain Point

Delivery itineraries are randomly assigned to each delivery driver upon reaching the delivery collection station. The delivery points are automatically generated and sorted using Amazon's routing algorithm. Drivers are allowed to change the sequence of delivery as and when they like.

As such, drivers has resorted to using applications like Circuit which allows them to key in their delivery points, and both their start and end points. The itinerary is optimized for them accordingly.

However, the downside of such apps is that they're generally limited in terms of the number of delivery points and it is also rather time consuming to key each delivery point individually.

# Solution

This Telegram bot attempts to address the shortfall by providing a free and easy alternative to delivery routing using OCR and Google Maps API. The user is required to define the following: Start and End Point, Screenshots of the itinerary screens.

The bot uses Google Maps Routes to optimize the amount of time required to deliver the goods. This provides time savings of more than 10% on average.

# Limitations
Google Maps API sets a 23 waypoint limit to their API calls. We will eventually address it in a future revision.

# Current Implementation:

Try not to abuse the limits set by the bot!
https://t.me/amapflexbot_bot