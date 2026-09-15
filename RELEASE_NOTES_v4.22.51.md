# Catered Cottage Healthcare v4.22.51

This is a bug-recovery release following the v4.22.50 mobile reports. The main failure was a startup JavaScript scope exception during bundled nursing-data initialization. That exception stopped later initialization code, which explains the Prepared Shift panel remaining on **Checking…** and DSD tools appearing nonfunctional.

The offending dependency has been removed from the cross-module startup path. Browser-style regression checks now show Prepared Shift resolving normally, the DSD Shift Planner opening, and the Facility Staffing / Sign-In Sheet opening from the planner.

The Nursing Directory mobile modal was also tightened so its own content scrolls while the header/footer remain available, with the app bottom action bar hidden behind open dialogs.
