<h1 data-path-to-node="0">Sports Management System Database Design</h1><h2 data-path-to-node="1">Project Overview</h2><p data-path-to-node="2">This database architecture is designed to manage the core operations of a sports organization, focusing on the coordination of teams, player rosters, match scheduling, and support staff. The system utilizes an <b data-path-to-node="2" data-index-in-node="210">Enhanced Entity-Relationship (EER)</b> model to ensure data integrity and clear accountability across all organizational levels.</p><h2 data-path-to-node="3">Data Architecture &amp; Entities</h2><h3 data-path-to-node="4">Core Entities</h3><ul data-path-to-node="5"><li><p data-path-to-node="5,0,0"><b data-path-to-node="5,0,0" data-index-in-node="0">Teams</b>: Tracks <code data-path-to-node="5,0,0" data-index-in-node="14">TeamID</code> (Primary Key), name, city, and coach.</p></li><li><p data-path-to-node="5,1,0"><b data-path-to-node="5,1,0" data-index-in-node="0">Players</b>: Stores athlete profiles, including a composite name (First, Middle, Last), contact information, position, and contract duration.</p></li><li><p data-path-to-node="5,2,0"><b data-path-to-node="5,2,0" data-index-in-node="0">Matches</b>: Manages match logistics, including date, location, and the identification of Home and Away teams via Foreign Keys.</p></li></ul><h3 data-path-to-node="6">Support &amp; Financial Entities</h3><ul data-path-to-node="7"><li><p data-path-to-node="7,0,0"><b data-path-to-node="7,0,0" data-index-in-node="0">Referees</b>: Records officiating personnel with unique IDs and phone numbers.</p></li><li><p data-path-to-node="7,1,0"><b data-path-to-node="7,1,0" data-index-in-node="0">Medical Staff</b>: Captures medical roles and their dedicated team assignments.</p></li><li><p data-path-to-node="7,2,0"><b data-path-to-node="7,2,0" data-index-in-node="0">Sponsors</b>: Manages external partnerships, tracking sponsor type and contact details.</p></li></ul><h2 data-path-to-node="8">Relationship &amp; Cardinality Rules</h2><p data-path-to-node="9">The model defines specific business logic to maintain structure within the organization:</p><div class="horizontal-scroll-wrapper"><div class="table-block-component"><response-element class="" ng-version="0.0.0-PLACEHOLDER"><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!----><!---->

Relationship | Cardinality | Business Logic

Team ↔ Match | m:m | Many teams participate in many matches.

Referee ↔ Match | 1:1 | One referee is assigned to one match and vice versa.

Team ↔ Player | 1:m | One team has many players, but each player belongs to only one team.

Team ↔ Medical Staff | 1:m | One team is served by many medical staff members.

Team ↔ Sponsor | 1:m | One team can have many sponsors.


</div><div _ngcontent-ng-c328199455="" hide-from-message-actions="" class="table-footer hide-from-message-actions ng-star-inserted"></div></div></table-block></response-element></div></div>
