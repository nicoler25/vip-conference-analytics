## VIP Conference Analytics | SQL Joins & Subqueries Case Study

## Executive Summary

This SQL case study analyzes a fictional VIP conference dataset to uncover attendance trends, hotel reservation patterns, RSVP behavior, peer feedback relationships, and data quality gaps.

Using PostgreSQL, I joined multiple relational tables to answer business questions related to event planning, attendee follow-up, hotel coordination, and operational reporting.

## Business Problem

Conference organizers need accurate attendee, reservation, RSVP, and relationship data to support planning decisions. This project uses SQL to identify:

* Events with the highest attendance
* VIPs missing reservation records
* RSVP trends for welcome and dinner events
* Hotel reservation volume
* Data mismatches between attendee and reservation records
* Peer feedback relationships between VIPs

## Tools Used

* SQL
* PostgreSQL
* Excel
* GitHub

## Dataset Overview

This project uses four relational tables:

* vips — VIP attendee details, assigned events, association type, membership year, and peer feedback relationships
* reservations — Hotel reservation details and RSVP status
* events — Conference event names and event types
* hotels — Hotel names and address information

Dataset includes: 30 VIP members, 30 reservation records, 12 events, and 3 hotels.

## Business Questions

1. Which events had the highest attendance?
2. Which VIPs had hotel reservations?
3. Which hotel had the most reservations?
4. Which attendees RSVP’d to the welcome event, dinner, or both?
5. Which VIPs were connected through peer feedback relationships?
6. Were there any data quality gaps between VIP and reservation records?

## SQL Techniques Used

* INNER JOIN
* LEFT JOIN
* SELF JOIN
* Multiple table joins
* Subqueries
* Aggregations
* Data validation checks

## Key Business Findings

* Events 2, 4, 6, and 7 had the highest attendance, with 3 attendees each.
* Marriott had the highest hotel reservation volume.
* 17 attendees RSVP’d yes to both the welcome event and dinner.
* 6 VIPs were not assigned to an event.
* 3 VIPs did not have matching reservation records.
* 3 reservation records did not match a VIP in the attendee table.
* Peer feedback relationships showed connections between VIP attendees.

## Data Validation Findings

The analysis identified several data quality gaps that could impact planning:

* VIP attendees without reservation records
* Reservation records without matching VIP records
* VIPs not assigned to an event
* RSVP differences between welcome event and dinner attendance

These gaps could affect hotel coordination, guest follow-up, seating, meal planning, and attendee experience.

## Project Visuals
![Attendees by Event](images/attendees-by-event.png)
![Reservations by Hotel](images/reservations-by-hotel.png)
![RSVP Breakdown](images/rsvp-breakdown.png)

## Business Recommendations
Based on the analysis, conference organizers could:
1. Prioritize resources for events with the highest attendance.
2. Follow up with VIPs missing reservation records.
3. Review unmatched reservation records for possible data entry issues.
4. Use RSVP trends to improve meal planning and event capacity estimates.
5. Use peer feedback relationships to identify highly engaged VIPs.
6. Maintain centralized attendee and reservation tracking to improve data accuracy.

## Final Summary
This project demonstrates how SQL can be used to analyze relational event data, identify operational trends, and uncover data quality issues. The findings support better conference planning, attendee follow-up, hotel coordination, and future event strategy.

## Skills Demonstrated
* SQL joins and subqueries
* Relational database analysis
* Data validation
* Aggregations
* Operational reporting
* Business analysis
* Data storytelling
* Business recommendations

## Next Steps
Future improvements could include:
* Building an interactive dashboard for attendance, reservations, RSVP behavior, and data quality
* Adding check-in status, event cost data, or post-event survey results
* Creating KPIs such as RSVP rate, reservation completion rate, and event engagement score
