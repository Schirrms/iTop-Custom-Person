# iTop-Custom-Person
## Some small customization to Person Class

At first, I built that extension only to change a little the uniqueness rule on the employee_number, as for our corporation, the employee_number '0000000' can be a duplicate.

I maybe could have to add other things 😊

OK, Just added the loginname, witch is normally used for iTop user. But here, it's a very good synchronization key for person also :)

## New in version 0.1.0

add a 'uid' field only for our synchronisation (that is, the field in not on display, but can be seen if someone modify a 'list view', it's not so secret !).
This field is at the 'person' Level.

add a 'dn' field, as our source is now Microsoft AD, and the dn is the ultimate link between Teams and Person. This field is add on a Contact level and is displayed on both Team and Person.

Also, in the link table between person and team (lnkPersonToTeam) a new field 'team_in_team' (text field), supposed to display the hierarchical link betwenn teams (hopefuly!).


# Installation

As for all my extensions, just download the zip file, and copy the 'schirrms-...' directory in your extensions directory, then rerun the setup as usual.