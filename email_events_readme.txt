Email Opened: Event fires when a user opens an email (we already have this; everything is all good)
	user_id: User/subscriber ID from our backend
	campaign_id: Campaign ID from our backend
	subject: Subject line of email
	template: Template of email

Link Clicked: Event fires when a user clicks on a link within the email
	url: URL the user is directed to
	img: Image file of the click
	headline: Headline in the email
	is_featured: Is it the featured article?

Follow Clicked: Event fires when a user clicks on one of our follow buttons
	action_type: FB, Pinterest, Twitter, Insta, Youtube will be args
	position: Top or bottom of the email

Nav Clicked: Event fires when a user clicks on one of our "menu" buttons at the bottom of the email
	section_clicked: Help, Contact, About, etc

Ad Unit Clicked: Event fires when a user clicks on one of the ads within the email
	position: Top, middle, or bottom ad
	creative: If possilbe, the image used

EOP Clicked:
	url: URL the user is directed to
	partner: Name of partner user is directed to
	img: Image file of the click
	headline: Headline for the article

Unsubscribed: Event fires when a user clicks on the unsubscribe button
	unsubscribed: Was unsubscribed clicked?

