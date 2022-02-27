# Texas-Inspection-Station-Locator
An overkill solution whose main purpose is to learn more about machine learning and if we can apply a complex solution to solve a simple problem.

## Problem: 

As a new resident to Texas, there are certain things you need to do in order to get your state license. One of those things is to get your vehicle inspected.

The official site at https://www.dps.texas.gov/rsd/vi/VIactiveStationLocator/viSrchResults.aspx only searches inspection stations based on: Zip Code, City, and County. It returns results in an undeterminate order (alphabetical?) and does not allow to filter interest types (annual, autocycle, electric vehicle, trailer, etc).

It does not take into account where you are relative to each station's location. This means you'd have to manually go through the list address by address to find one that is closest to **you**. Most will either indiscriminately pick the first one on the list, or use Google Maps to find one closest to them, rendering this site useless. Google cannot be a reliable source if you're not including the right keywords or if the business themselves have forgotten to register their business as having inspections as a service.

## Proposed Solution:

Provide a form/site where users can enter their address or pin drop shared from Google Maps and have it spit out a list of stations that best fit their promixity for them to pick and choose.

### Challenge:

Try to reduce use of API calls to services that can otherwise calculate distance calculation for us as it would have to iterate through the entire list to find most optimal path, resulting in service cost.

## Alternatives:

Use Euclidean distance to calculate the distance between two points, after having gathered all the points.

## Potential Bonus Benefits:

Models can be trained using coordinates in addition to street names and over time would rely less on API external calls as it can make a guess of what it has seen before.
