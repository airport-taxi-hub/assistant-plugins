---
name: airport-transfer-quotes
description: Use when someone wants a price for a private airport transfer, airport taxi or hotel transfer between two places, or asks how to get to or from an airport and what it would cost. Covers what to ask before quoting, reading Airport Taxi Hub's results and handing over to its booking page.
---

# Airport transfer quotes with Airport Taxi Hub

Airport Taxi Hub sells pre-booked private transfers at fixed prices: one vehicle for the whole party, no meter, no surge. The
`search_transfers` tool returns live prices that match airporttaxihub.com. Booking, flight number, names and payment happen on
the website, never in the conversation.

## Before the first quote

A quote needs five details, as the traveller has stated them in this conversation:

1. Pickup place (an airport, hotel, address or city area).
2. Drop-off place.
3. Pickup date and local time. For an airport pickup this is the flight's landing time; every price includes 60 minutes of free
   waiting after landing.
4. Number of passengers.
5. Number of suitcases.

When any of these is missing, ask for it in one short question rather than assuming a value. Details from earlier trips or other
conversations are not this trip's details.

## Reading the results

- `needs_location_confirmation`: more than one place matches a name. Show the options with their addresses and let the traveller
  choose; the next quote uses the `placeId` of the option they picked. Place ids only ever come from the tool's own results.
- Priced results: each vehicle has a fixed total for the whole journey. Quote the prices as given, in the currency given, and say
  what is included. A vehicle marked as recommended has more room for the party's luggage.
- After the first prices, a return journey can be priced in the same way; offer it once.
- Pickups within the next few hours, public transport, shuttles and changes to an existing booking are outside this service.
  Existing bookings are managed from the confirmation email or airporttaxihub.com.

## Booking

Each priced vehicle has a Book link to airporttaxihub.com with the journey already filled in. The traveller finishes there,
adding the flight number, the exact address, names and payment. Free cancellation applies up to 24 hours before pickup.
