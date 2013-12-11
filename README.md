airport-delays
==============

A simulation of the US air traffic network with a shortest-path finder for flights (based on linear regression and Dijkstra's algorithm), and a KML heat map generator.

## Notes

- To operate this code, you will need to download the SQLite database of flights we prepared (approximately 7GB in size). Due to size limitations, this is not currently stored online for public download. If the status of this changes, we will update this README with its location.

## Useful Information
Flight Database Schema:
CREATE TABLE FlightTest(RowID integer primary key asc, Year integer, Quarter integer, Month integer, DayofMonth integer, DayofWeek integer, FlightDate text, UniqueCarrier text, AirlineID integer, Carrier text, TailNum integer, FlightNum integer, OriginAirportID integer, OriginAirportSeqID integer, OriginCityMarketID integer, Origin text, OriginCityName text, OriginState text, OriginStateFips integer, OriginStateName text, OriginWac integer, DestAirportID integer, DestAirportSeqID integer, DestCityMarketID integer, Dest text, DestCityName text, DestState text, DestStateFips text, DestStateName text, DestWac text, CRSDepTime integer, DepTime integer, DepDelay integer, DepDelayMin integer, DepDel15 integer, DepartureDelayGroups integer, DepTimeBlk text, TaxiOut integer, WheelsOff integer, WheelsOn integer, TaxiIn integer, CRSArrTime integer, ArrTime integer, ArrDelay integer, ArrDelayMin integer, ArrDel15 integer, ArrivalDelayGroup integer, ArrTimeBlk integer, Cancelled integer, CancellationCode text, Diverted integer, CRSElapsedTime integer, ActualElapsedTime integer, AirTime integer, Flights integer, Distance integer, DistanceGroup integer, CarrierDelay integer, WeatherDelay integer, NASDelay integer, SecurityDelay integer, LateAircraftDelay integer, FirstDepTime integer, TotalAddGTime integer, LongestAddGTime integer, DivAirportLandings integer, DivReachedDest integer, DivActualElapsedTime integer, DivArrDelay integer, DivDistance integer);
