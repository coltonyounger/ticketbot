12/30/24 Version 1.0 for Booking Bot and Ballroom Ticketbot.

  Booking Bot is a bash script that links to the ticket booking site tabletop.events and attempts to add an attendance badge to a cart for a sold out convention. 
  Two badge types are available and each type is targetted by the bash script every second per the website API's documented best practices. Output is written to a 
  text document to verify the proper errors are being returned ("Badge is out of stock.") instead of unforseen problems. Note the current convention currently in 
  use has already passed at the beginning of December and different API calls need to be made for convention_id and badgetype_id parameters.

  Ballroom Ticketbot is a bash script very similar to Booking Bot but requires a badge already acquired for the specific convention and attempts to add an exclusive 
  event to the badge happening at the convention. Spots for these events were similarly sold out but had five different types instead of two for the original ticketbot 
  and also connects through the API every second.
