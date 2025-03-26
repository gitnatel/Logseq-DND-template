### Session
template:: Session
template-including-parent:: false
collapsed:: true
	- ### World Information
		- Start Date:
		- Start Location:
	- ### Plan
	- ### Notes
	- ### EOS Checklist
		- Days Passed:
		- Session Summary
			-
-
- ### Character (Player)
  template:: Character (Player)
  template-including-parent:: false
  collapsed:: true
	- type:: Character (Player)
	  name::
	  race::
	- ### Description
	- ### Relationships
	- ### Personal Quests
	- ### Character Sheet
	- ### Notes
-
- ### Character (NPC)
  template:: Character (NPC)
  template-including-parent:: false
  collapsed:: true
	- type:: Character (NPC)
	  name:: 
	  race::
	  faction::
	  location::
	- ### Description
	- ### Relationships
	- ### Motives
	- ### Stat Block
	- ### Quests
		- {{query (page-property :questgiver <%current page%>)}}
	- ### Notes
-
- ### Location (Region)
  template:: Location (Region)
  template-including-parent:: false
  collapsed:: true
	- type:: Location (Region)
	  name::
	  parent_location::
	- ### Description
	- ### Map
	- ### Sub-Locations
		- {{query (page-property :parent-location <%current page%>)}}
	- ### Historical Events
		- {{query (and (page-property :location <%current page%>) (page-property :type "Historical Event"))}}
	- ### Notes
-
- ### Location (Specific)
  template:: Location (Specific)
  template-including-parent:: false
  collapsed:: true
	- type:: Location (Specific)
	  name::
	  location-type::
	  parent-location::
	- ### Description
	- ### Map
	- ### Sub-Locations
		- {{query (page-property :parent-location <%current page%>)}}
	- ### NPC's
		- {{query (and (page-property :location <%current page%>) (page-property :type "Character (NPC)"))}}
	- ### Factions
		- {{query (and (page-property :location <%current page%>) (page-property :type "Faction"))}}
	- ### Quests
		- {{query (and (page-property :location <%current page%>) (page-property :type "Quest"))}}
	- ### Encounters
		- {{query (and (page-property :location <%current page%>) (page-property :type "Encounter"))}}
	- ### Historical Events
		- {{query (and (page-property :location <%current page%>) (page-property :type "Historical Event"))}}
	- ### Notes
-
- ### Faction
  template:: Faction
  template-including-parent:: false
  collapsed:: true
	- type:: Faction
	  name::
	  leader::
	  location::
	- ### Description
	- ### Motives
	- ### NPC's
		- {{query (and (page-property :faction <%current page%>) (page-property :type "Character (NPC)"))}}
	- ### Notes
-
- ### Encounter
  template:: Encounter
  template-including-parent:: false
  collapsed:: true
	- type:: Encounter
	  name::
	  location::
	  trigger::
	  parent-quest::
	- ### Description
	- ### Loot
	- ### Notes
-
- ### Creature
  template:: Creature
  template-including-parent:: false
  collapsed:: true
	- type:: Creature
	  name::
	  creature-type::
	- ### Description
	- ### Stat Block
	- ### Notes
-
- ### Item
  template:: Item
  template-including-parent:: false
  collapsed:: true
	- type:: Item
	  name::
	  item-type::
	- ### Description
	- ### Stat Block
	- ### Notes
-
- ### Quest
  template:: Quest
  template-including-parent:: false
  collapsed:: true
	- type:: Quest
	  name::
	  questgiver::
	  location::
	- ### Description
	- ### Encounters
		- {{query (page-property :parent-quest <%current page%>)}}
-
- ### Historical Event
  template:: Historical Event
  template-including-parent:: false
  collapsed:: true
	- type:: Historical Event
	  name::
	  location::
	  date::
	- ### Description
	- ### Notes
-
- ### Miscellaneous
  template:: Miscellaneous
  template-including-parent:: false
  collapsed:: true
	- type:: Miscellaneous
	  name::
	- ### Description
	- ### Notes