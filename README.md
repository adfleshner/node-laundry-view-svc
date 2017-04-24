This is a fork of Nixta's wonderful library [node-laundry-view-svc](https://github.com/nixta/node-laundry-view-svc). Altered a bit to work this the university of Alabama's Laundry View Syste. I take no credit in writing any of this all I did was find where he was loading his campus and change it to the one I wanted. The code works awesome. https://ua-laundry.herokuapp.com/

node-laundry-view-svc
=====================

An ExpressJS server providing JSON output for current Laundry Room statuses in Stuyvesant Town.

See it live at [http://st-laundryview.herokuapp.com/rooms](http://st-laundryview.herokuapp.com/rooms).

Individual rooms are under the `/room/<roomId>` resource path. E.g. [http://st-laundryview.herokuapp.com/room/4335325](http://st-laundryview.herokuapp.com/room/4335325).

The original resident access page can be found [here](http://www.laundryview.com/lvs.php?s=219) (expand an address, and click on the revealed identical address to see a Flash animation of the availability).

## Notes
A room is not loaded until required. It is then cached for 60 seconds. Requests within the next 60 seconds do not hit the original data source.
