### Regions
	- {{query (page-property :type "Location (Region)")}}
	  query-properties:: [:name :parent-location :created-at :updated-at]
-
- ### Specifics
	- {{query (page-property :type "Location (Specific)")}}
	  query-properties:: [:name :location-type :parent-location :created-at :updated-at]
	  query-sort-by:: updated-at
	  query-sort-desc:: false