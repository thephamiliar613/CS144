Part B: Design your relational schema
1. 	Items
		(ItemID*, Name, Currently, Buy_Price, First_Bid, Number_Of_Bids, LocationName, Latitude, Longitude, Country, Started, Ends, SellerID^, Description)
	Category
		(ItemID^*, Category*)
	Bids
		(BidderID^*, ItemID^*, Time*, Amount)
	Users
		(UserID*, BidderRating, SellerRating, Location, Country)

	*primary keys
	^foreign keys

2.	Items.ItemID -> Name, Currently, Buy_Price, First_Bid, Number_Of_Bids, LocationName, Latitude, Longitude, Country, Started, Ends, SellerID, Description
	Category.ItemID -> Category
	Bids.BidderID, Bids.ItemID, Bids.Time -> Amount
	Users.UserID -> BidderRating, SellerRating, Location, Country

3. Yes
4. Yes