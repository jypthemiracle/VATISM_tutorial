# S1 Course Lecture II - Meteorology and Altimetry

## METAR & SPECI

* **METAR**
  * A routine weather report issued at hourly or half-hourly intervals.
  * A description of the meteorological elements observed at an airport at a specific time.
  * observed 10 minutes before rendering a report

* **SPECI**
  * A special weather report issued when there is an significant deterioration or improvement in weather conditions.
  * similiar to METAR
* Format
  * Airport (ex. VHHH for HK)
  * Observation time
  * Wind at ground level: direction, speed, unit (knots)
  * Meteorological visibility
  * Runway Visual Range(RVR) if visibility is below 1500m.
  * Present Weather
  * Clouds, amount, type and base
  * Air temperature and dew point
  * QNH (air pressure)
  * Other information (ex. wind change)
  * Landing forecast, trend.
  * get familiar with codes
  * **Example**
    * METAR
    * VHHH - ICAO code
    * 121755Z - Date and time (December 17, 17:55 in UTC time(Z))
    * 21016G24KT - wind comes 210 degrees at 16 knots, gusting to 24 knots
    * 180V240 - wind direction is variable between 180 degrees to 240 degrees
    * 1500 - 1500 meters for prevailing visibility.
    * R07R/0600U - Runway visibility. 600 meters improving(U). D stands for decreasing values.
    * RA - rain / BR - mist
    * BKN015 OVC025
      * shows the amount of sky cover and cloud base height.
      * in 1500 feet, cloud covers 4/8 till 7/8(BKN).
      * in 2500 feet, cloud overcasting at the height.
    * 06/04
      * TEMP and DEW POINT
      * temperature: 6 degrees
      * dew point: 4 degrees
    * Q1005
      * atmospheric pressure measure at ground level
      * 100.5 헥토파스칼
    * BECMG 999=
      * TREND
      * How weather is going to develop in that time the METER is current(2 hours).
      * TEMPO = Temporary change in weather
      * BECMG = Permanent change in weather

## Wind

* 10 minutes average
* given in knots(kt)
* more than 60 degrees and more than 3kt wind, V (variable)
* less than 3kt wind and it varies, reported as VRB.
* Calm = 00000KT
* Example
  * VRB02KT = variable 2 knots
  * 25020KT  = two five zero degrees two zero knots
  * 15015G25KT = one five zero degrees one five knots gusting two five knots
  * 24018G35KT 160V290 = two four zero degrees one eight knots gusting three five knots variable between 160 degrees and 290 degrees

## Ground Visibility

* visibility up to 10km.
* below 50m is 0000
* above 10km is 9999

## Runway Visual Range

* RVR only measured if visibility is below 1500m.
* starts with R by the runway designator but if there is more than one runway in the same direction, L(left), R(right), C(center) are used.
* M: below 50m
* P: more than 1500m
* V: varies
* U: going up
* D: going down
* Examples
  * R29L/0700 - R-V-R two niner left, seven zero zero meters
  * R19R/M0150D - R-V-R one nine niner right, below one five zero meters going down
  * R26/0350V06000U - R-V-R two six variable between three five zero and six zero zero meters going up

## Weather Phenomena

* VC means vicinity, which means within 8 km from the airport.
  * exception: thunder and cumulonibmus clouds.
* SN BLSN - snow and blowing snow
* FZDZ FG - heavy freezing drizzle with fog
* RESN - recent snow

## Clouds

* Cumulonimbus(CB) - 적란운

![Sky Timelapse of Cumulonimbus Clouds with Lightning - YouTube](https://i.ytimg.com/vi/KVTs2DQoSrE/maxresdefault.jpg)

* Towering Cumulus(TCU) - 웅대적운

![Cumulus congestus cloud - Wikipedia](https://upload.wikimedia.org/wikipedia/commons/f/f4/Cumulus_congestus_cloud.jpg)

* Otherwise, the sky covered by clouds is measured
* 0/8 - SKY CLEAR SKC
* 1~2/8: Few FEW
* 3~4/8: Scattered SCT
* 5~7/8: Broken BCT
* 8/8: Overcast OVC
* The cloud base above the airport's reference height
* AGL(Above Ground Level) is measured in hundreds of feet. 001 means 100ft, 012 means 1200ft, 120 means 1200ft.
* Vertical visibility = VV if not VV//
* Examples
  * BKN002 - Broken two hundred feet
  * SCT013 BKN120 - Scattered one thousand three hundred feet. Broken one two thousand feet.
  * SCT035TCU - Scattered three thousand five hundred feet, towering cumulus

## CAVOK

* replaces visibility if no CB/TCU/precipitation/cloud below 5000ft and more than 10km visibility.
* Clouds and Aviation OK

## Temperatures and Dew Point

* degrees Celsius
* Dew point
  * temperature the air must be cooled to get saturation (ex. relative humidity 100%)
  * indicates the risk of ice formation.
* The closer the temperature and dew point are, the more humidity is in the air and the worse is the visibility.
* Spread
  * The difference between temperature and dew point
* Lowest cloud base
  * SPREAD * 400ft.
* M: below 0
* Examples
  * 02/M04: Temperature two dew points minus four

## Trend

* indicate change within next two hours.

* Becoming BECMG
* Temporary TEMPO
* No Significant Change (stable) NOSIG
* The first two can be given with a time reference.
* Examples
  * BECMG FM1250 TL1340
    * becoming from 1250 till 1340, the change will take place between 12:50 and 13:40
  * BECMG AT 1400
    * the change will take place at 1400
  * TEMPO FM 1400
    * one or more temporary changes shorter than one hours, from 14:00 to two hours after the METAR was reported.

## Runway Conditions

* when affecting aircraft's landing and departing.

## VMC and IMC

* **Visual meteorological conditions** (**VMC**) : allowing conditions in that [visual flight rules](https://en.wikipedia.org/wiki/Visual_flight_rules) (VFR) flight is permitted—that is, conditions in which [pilots](https://en.wikipedia.org/wiki/Aviator) have sufficient visibility to fly the [aircraft](https://en.wikipedia.org/wiki/Aircraft) maintaining visual separation from terrain and other aircraft. They are the opposite of [instrument meteorological conditions](https://en.wikipedia.org/wiki/Instrument_meteorological_conditions) (IMC). The boundary criteria between IMC and VMC are known as the VMC minima and are defined by: [visibility](https://en.wikipedia.org/wiki/Visibility), cloud ceilings (for [takeoffs](https://en.wikipedia.org/wiki/Takeoff) and [landings](https://en.wikipedia.org/wiki/Landings)), and cloud clearances.
* **Instrument meteorological conditions** (**IMC**) describes weather conditions that require pilots to fly primarily by reference to instruments, and therefore under [instrument flight rules](https://en.wikipedia.org/wiki/Instrument_flight_rules) (IFR), rather than by outside visual references under [visual flight rules](https://en.wikipedia.org/wiki/Visual_flight_rules) (VFR). 
  * Typically, this means flying in [cloudy](https://en.wikipedia.org/wiki/Cloudy) or bad [weather](https://en.wikipedia.org/wiki/Weather). Pilots sometimes train to fly in these conditions with the aid of products like [Foggles](https://en.wikipedia.org/wiki/Foggles), specialized glasses that restrict outside vision, forcing the student to rely on instrument indications only.

## Terminal Aerodrome Forecast(TAF)

* providing a prediction of the weather conditions within 5 statue miles of the aerodrome normally for next 24 hours period.

## AIRMET and SIGMET

* AIRMET - Airmen's Meteorological Information
  * referred to as Weather Advisories
  * valid for 4 hours for all aircraft
  * AIRMET SIERRA(Mountain obscuration or IFR)
    * celling less than 1000 feet
    * visibility less than 3 miles affecting over 50% of the area at one time
    * extensive mountain obscuration
  * AIRMET TANGO(Turbulence)
    * Light, moderate turbulence, sustained surface winds of 30 knots or more
  * AIRMET ZULU(icing)
    * Light, moderate icing, freezing levels
* SIGMET - Significant Meteological Information
  * Concerning non-convective(비대류의) weather that may affect safety of ALL aircraft
  * include severe icing not associated with thunderstorms, severe or extreme turbulence or clear air turbulence (CAT) not associated with thunderstorms, dust storms or sandstorms that lower surface or inflight visibilities to below 3 miles and volcano ash.
  * valid for 4 hours usually

## PIREP

* Pilot's report but not prevalent one.
* conditions as they exist in the air, which cannot be gathered from any source.
* pilots can confirm the height of bases.. and so on.

## Air Pressure and Temperature

* static pressure = pressure that the atmosphere is producing which is measured in hectopascal(hPa).
* Air gets thinner with increased altitude (30 hPa/1000 ft)
* Aircraft altimeter uses this variation of air pressure around the aircraft to display altitude.
* QNH - air pressure that measures above sea level.
* Standard Lapse Rate: The temperature drops 2 degree per 1000 ft in standard atmosphere.

## Altitude and Height

* Altitude: vertical distance between mean sea level (MSL) and an aircraft.
* height: vertical distance between the GND or an airport and an aircraft.
  * i.e) If an aircraft is flying on altitude 1000ft while the airports' elevation (which means height above MSL) is 300ft, the aircraft height is 700ft.

## Flight Level

* When controlling a pilot's aircraft, an air traffic controller can give an instruction to change the aircraft altitude.
* QNH: Atmospheric pressure at mean sea level
* QFE: Atmospheric at a specified datum such as airfield runway threshold.
* Why it is needed:
  * http://blog.daum.net/insburg/3740610
  * https://m.blog.naver.com/rits/55958753

https://mediawiki.ivao.aero/index.php?title=Altimetry_for_air_traffic_controller

#### Climbing Phase

![Altimetry TA TRL climbing.png](https://mediawiki.ivao.aero/images/d/d2/Altimetry_TA_TRL_climbing.png)

#### Descending Phase

![Altimetry TA TRL descending.PNG](https://mediawiki.ivao.aero/images/4/44/Altimetry_TA_TRL_descending.PNG)