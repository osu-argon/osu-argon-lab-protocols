# Leak Testing on Mass Spectrometers

## ID

`leak_test`

## Requires

`rate_of_rise`

## Description

If there is a potential leak in a mass spectrometer it is best to systemically rule out locations for the leak. In general you start with a rate of rise and systemically open up and close valves until you think you have found the general location of the leak. At that point you will need Argon gas to spot check locations within that region.

## Procedure

1. Perform `rate_of_rise` until it become clear where the general area of the leak is coming from.
2. Use Argon to test seals in the suspected area.
3. If the leak is small it make take a few minutes for the argon to make it's way into the system. Spend around 4 minutes in each area.
4. If there is a leak, there will be a spike in m40.

