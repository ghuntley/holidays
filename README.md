# Holidays

# Specification
* MUST be cross platform (Windows/Mono/Xamarin) by default.
    * Thus be a Portable Class Library
* Data MUST be automatically generated from upstream source to reduce maintenance burden on maintainers and defect possibilities.
    * Thus use https://github.com/alexdunae/holidays as upstream data source.


# API Design
* There are three types of holidays (Holiday, Observed and Informal)
   * Holiday = ANZAC Day
   * Observed = Canada Day
   * Informal = Valentine's Day

## Get holidays on a specified date

    Holidays.On(DateTime, [Region|Regions], [HolidayType|HolidayTypes](Holiday|Observed|Informal))
      => List<string>
         => ANZAC Day

    - Should we return null on no results or empty list - ie. Holidays.On(parms).Any()

## Get holidays observed on a specified date
## Get informal holidays on a specified date
## Determine if a specified date is a holiday

# Usage

To install all regions:

    Install-Package Holidays

To install a specific region:

    Install-Package Holidays.Australia
    Install-Package Holidays.UnitedNations
    Install-Package Holidays.NYSE

