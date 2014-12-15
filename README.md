# Holidays

# Specification
* MUST be cross platform (Windows/Mono/Xamarin) by default.
    * Thus be a Portable Class Library
* Data MUST be automatically generated from upstream source to reduce maintenance burden on maintainers and defect possibilities.
    * Thus use https://github.com/alexdunae/holidays as upstream data source.

# Usage

To install all regions:

    Install-Package Holidays

To install a specific region:

    Install-Package Holidays.Australia
    Install-Package Holidays.UnitedNations
    Install-Package Holidays.NYSE

