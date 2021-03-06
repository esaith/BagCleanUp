 Special Thanks To:
  Stepphy - Nathezrim for the initial tester. You helped modify the original architecture from dependent on default bags to allowable of all bag addons
  JuniorDeBoss - For helping me out with tooltip bugs and reducing spamming number
  Podden - For helping me out with additional tooltip bugs from (possibly) other addons that have extensive tooltip use
  Guild Master - Feedback on overall product
  _Max_Cavalera_ - For the suggestion to adding an option to keep all BOE when picking up. This is the "Keep All BOE" option on the Options page
 
  1.38
	Update for BFA 8.0
	Reverted Hitem to link

	Added Features
		Added character list on options panel to toggle which characters to view when viewing saved dungeons.
		When 'Do not sell Uncommon or Trade Goods', the alpha should be apparent as if the user manually click the item. The item is not included on the kept list, though

	Fixed Issues
		Fixed scrolling on Raid Info list. When scrolling with the mouse wheel, the scroll nob scrolls as well
		After closing the options tab, the bottom tab now shows the items tab correctly instead of defaulting to Raid Info tab

  1.37
	Update for 7.3. 
	Significant code update.
		Changed saving items from 'link' to 'Hitem'
	
	Added/Updated Features
		After user selects an option from a drop down, the selected item is now saved as the new drop down title 
		All gear currently worn is automatically added to the players kept list. This should provide additional security that items should not be sold. 
		
		Raid Info
			User may now filter this list to view which characters are saved to which instance. This is provided in the options panel
			Saved instances are now in a tabular format instead of string based.
			If no instances are chosen then a info message lets the user know where to update this list.

	Removed Items
		iLevel fitler
		Removed artwork background. Images are cool but deters from actual use of Addon
		Removed background colors for items. Should be reintroduced after Hitem fix
		BOE section removed. Should be reintroduced after Hitem fix
	
	Known Issues
		Scrolling on Raid Info raw list with middle mouse does not update scroll position
		Occasionally items are not shown properly per zone.
		After closing the options the bottom tab defaults to the Raid Info tab.
 1.36
	Fixed issue with variables from v1.32 to v1.36 This fixed the issue when selecting "Keep all BOE" option would cause LUA error
    Fixed issue when updating the AddOn to a higher version all instance and raid info would be erased.
    Fixed issue where hovering over non-link item (e.g. profession enchant that is not an item) an error would occur.


  1.35    
	Instances and player names are sorted alphabetically
	Fixed issue when one of the items is a pet would cause a popup error
    When opening options all other tabs, panels, buttons, etc that are not directly related to options is hidden. This should help reduce confusion of 
        which tab and information the player receives and then when attempting to navigate to another tab.
    Added "Quest Complete" which quickly obtains and completes quests. Excellent for leveling! Quest rewards are randomly chosen. 
    Added "Keep All BOE" checkbox. When checked every BOE of Uncommon quality (Green) or greater is immediately put in the kept list
    Prevents the "Item is busy" error from occurring when selling items
 
  1.34
     Updated for Legion expansion
	 Loot Frame
		 Added a loot frame so that looted items now appear in a separate frame than the main frame
		 Background of loot frame may be enabled/disabled. Enabled by default. If disabled a default of a black background is shown		
		 Background images change with each new session. Up to 50+ different images can be seen
		 The loot frame will have a minimum size close to that of the main frame. If the number of items start to exceed the size then the loot frame should increase in size so accommodate the number of items
		 All images are the property of Blizzard. None of them are the authors art work. These images are located inside the game client
	 Side tabs have been removed for a cleaner 1 page look
	 The options tab is now the cog-wheel located on the top right corner
	-Zone dropdown
		 Slight addition the way the dropped down works for zoning. If all items are desired, then the player must choose "ALL" to view the all items (replaces 3rd tab)
		 When selecting a zone/instance all filters are enabled. The player may now filter on zones
		 The capability to filter by iLevel is available. Off by default. The player may choose the to turn this option on in the options panel. Same filtering applies from prior version

 1.33
  Updated global variables to use local variables for easy writing and shorter lines of code.  
     Added Auto greed on green items 
	 Included background colors to selected filtered items to more easily distinquish which levels are which rarities
	 Increased the base height of the addon so that it doesn't jump as much when 
	 Moved the Do Not Sell Trade Goods to the options page. Now all filtering pages have that option.
		 When checkbox is marked all trade goods are added to a secondary saved list and become transparent like the normal trade goods. If Trade Goods becomes unmarked then all items will lose their transparency unless they are saved by the manual toggle (normal kept list)
	 When Reset now does not reload the game. 
	 Included items that don't have 'bind on pickup', 'bind on pick up', or 'soulbound' in the item description. This should help with other items such as patterns 
	
 1.32
	 The issue with the tooltip looking funny while looting should now be resolved. The likely culprit is due to other addons that support and extend extensive tooltip options (multiple boxes). Since the BOE/BOP is checked by using the tooltip and that the tooltip is modified by using other addons, the tooltip is now hidden after reading.  

 1.31
     Fixed issue when getting items from the mailbox. The tooltip would look and act funny
     Added more detailed information to raid instances. This should help distinguish between 5 man dungeons with heroic and mythic availability

 1.3 
    Auto loot all containers. If room is not available a message is printed in the chat box.
       ** Currently this does not include salvage boxes, or any container that has a cast time.
     Make loot buttons smaller and increased the number per row
     Better fitting frame to number of items.
     Organzied items by rarity. Lowest quality up top, highest quality on bottom
     Added an options panel
     Added Coordinates to be turned off/on that is located under the mini-map
     Fixed issue where addon would appear to 'jump' when going from tab to the next
     Added Auto-sell junk items when first talking to a vendor
     Addon auto-updates internal variables when it recognizes its an older version that current installed. When updating any saved lists should still be saved
     Prevented addon from immediately opening when talking to a vendor (even the programmer got annoyed)
         Added button to Merchant Frame to toggle addon open/close
     Added auto addon update depending on its version.
     When scrolling over items a comparison to equipped items can be made by pressing any <Shift> button
     Added BOE section that removes all BOE items of rare (blue) quality or higher to the bottom of the list for easier filtering
         Included in options page to include green (if so desired)
     Added reset command line in case the user is unable to do from button

1.2 Moved the items options from the bag to the actual addon. Should reduce the chance of interfering with other bag addons or addons that do similar functions. Instead of seeing all items and then dimming those that 
 are wished to be sold, only the items will appear that contain to the selected tab - then the player may select the item to keep it on the list
 This list is updated once all items are sold; yet, if an item is added to the bags after selected checkboxs have marked then those items likely won't show up until the next change in checkboxes occurs.

1.1 Added tab #4, Player/Character Info. Reset Addon Button. View instance resets for all characters. For the character raids/instances to show they player only needs to log in 
 and is not required to open the addon. Only instances that have a heroic mode or higher and if the character is level 70 or higher

1.0 
 Initial Version 3 tabs (Zone, iLVL, Rarity). Allows mass auto-sell. 
 "Keep item" when addon is visible. ALT + Click item, blue haze adds item to auto-sellable list. Alt + Click again to unlink it