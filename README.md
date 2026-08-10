# FIA Driver Categorisation List — machine-readable copy

This repository holds a single file, `drivers.json`, containing the FIA Driver
Categorisation List in a form software can read.

## Unofficial

**This is an unofficial copy. It is not affiliated with, endorsed by, or
connected to the Fédération Internationale de l'Automobile.**

The FIA's own published list is the only authority on any driver's
categorisation. If this file and the FIA disagree, the FIA is right.

- Official list: <https://www.fia.com/fia-driver-categorisation>

The data itself belongs to the FIA. It is reproduced here because the FIA
publishes it publicly, and no claim of ownership over it is made.

## What is in the file

```
lastUpdated       the date this copy was taken
source            which FIA sources it was built from
driverCount       number of drivers in this file
drivers[]         one entry per driver
```

Each driver:

| Field | Meaning |
|---|---|
| `lastName`, `firstName` | as published by the FIA; `firstName` may be absent for drivers racing under a pseudonym only |
| `lastNameNote`, `firstNameNote` | text the FIA prints in brackets — usually a racing pseudonym, occasionally a date of birth where it is the only thing distinguishing two drivers of the same name |
| `searchAlias` | an alternative name, useful for searching, not intended for display |
| `nationality` | may be absent where the FIA prints none |
| `category` | `platinum`, `gold`, `silver` or `bronze`, or absent where a driver has no current grade |
| `underInvestigation` | the driver's categorisation is under review |
| `nextCategory`, `nextCategoryDate` | a grade taking effect on a future date |

## Accuracy

Every grade in this file is taken from the FIA's public categorisation feed and
independently cross-checked against the FIA's published PDF. Where the two
disagree, or where two drivers share a name and cannot be told apart, the
discrepancy is reviewed by hand before publication rather than resolved
automatically.

That said, mistakes are possible. Check anything that matters against the
official list.

## Updates

Updated by hand when the FIA publishes changes. `lastUpdated` in the file tells
you how current this copy is.
