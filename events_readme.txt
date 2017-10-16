#If an item appears in parentheses, programmatically add it
#ex. (Social) -> add pin or facebook
#If a property has —-, it does not appear but is included for reference
#ex. —-referral -> referral property deleted but kept for reference

Article Clicked: Event fires whenever someone clicks into an article, and they're already on the site.
	current_url: URL the user is currently on
	destination_url: URL the user is directed to
	element: Essentially 'class' (ex. "vertical-image" or "vertical-title")
	image_id: Either the source or backend ID for the image, if applicable
	position: Article index (if in a slideshow, for example)
	article_title: The actual (in the cms) title of the article
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name

(Social) Article Shared: Event fires when one of the "share" buttons is clicked.
	current_url: URL the user is currently on
	action_type: Args will be Facebook, Pinterest, Text, Email, Print
	position: Article index (if in a slideshow, for example)
	location: 'surround_article' or 'incontent', for example
	element: 'side' or 'stickynav', for example
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name

Follow: Event first when a user clicks on one of the “Follow” buttons
	current_url: URL the user is currently on
	action_type: Args will be Facebook, Insta, Pinterest, Snapchat, Twitter, YouTube
	location: Header, footer, or sidenav (pending class names)
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name

Article Completed: Event fires when a user reaches the end of an article.
	current_url: URL the user is currently on
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name

Slideshow Engaged: Event fires when a user clicks on any of the slideshow specific elements on the site.
	current_url: URL the user is currently on
	item_clicked: The URL of the article a user clicks (if applicable)
	slide_position: The furthest slide index the user reaches
	slide_exit: What slide index the user exits on
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name

Navbar Clicked: Event fires when a user clicks on one of the navbar elements.
	current_url: URL the user is currently on
	location: Explicitly either the "top" nav or the "side" nav
	element: fashion/beauty/recipes/home/family/how-tos OR lifestyle/trending/videos/cities
	subelement: null if location == top; child to element if location == side
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name

Footer Clicked: Event fires when a user clicks on any of the footer specific elements on the site.
	current_url: URL the user is currently on
	item_clicked: The URL of the article a user clicks (if applicable)
	element: 'privacy' or 'contests', for example
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name

(Referral) EOP Clicked: Event fires when a user clicks on one of the EOP elements on the site.
	current_url: URL the user is currently on
	destination_url: URL the user is directed to
	element: 'zergnet_03_ARGS' or 'purewow_04_ARGS', for example
	position: Article index (if in a slideshow, for example)
	—-referral: Args will be Internal, Zergnet, PubExchange (etc.)
	module_type: 'desktop_partner_category' or 'eop_slider', for example
	article_title: Article a user clicks to (ex. 'h4 class="slider__hed"')
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name

Right Rail Clicked:
	current_url: URL the user is currently on
	destination_url: URL the user is directed to
	element: 'zergnet_02', for example
	article_title: Article a user clicks to (in the hyperlink, as of 4/11/2017)
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name

Quiz Taken:
	current_url: URL the user is currently on
	questions_answered: Furthest question answered on the quiz
	result_viewed: Actual output of the result, if viewed
	quiz_retaken: Boolean quiz retaken or not
	quiz_shared: Where the quiz was shared to ('pin_quizresults_ARGS', for example)
	back_button_clicked: If the back button on the quiz (not in the browser) was clicked
	answers_given: Specific answers chosen on the quiz, returned as a demlimited string in one "cell"
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name
	
Pinterest Quiz Taken:
	current_url: URL the user is currently on
	questions_answered: Furthest question answered on the quiz
	pin_viewed: If the user went to Pinterest to see their pin; Bool
	quiz_retaken: Boolean quiz retaken or not
	quiz_shared: Where the quiz was shared to ('pin_quizresults_ARGS', for example)
	back_button_clicked: If the back button on the quiz (not in the browser) was clicked
	answers_given: Specific answers chosen on the quiz, returned as a demlimited string in one "cell"
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name

Recipe Box Engaged:
	current_url: URL the user is currently on
	recipe_added: Recipe that's added
	recipe_removed: Recipe that's removed
	recipe_printed: If a user prints the recipe
	social_share: If/where a user shares on social, email, or text
	add_more_recipes: If a user clicks the add recipes box
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name

Shop Module Engaged:
	current_url: URL the user is currently on
	module_position: Where the module itself appears
	item_clicked: '1_shopmodule_Topshop' or 'picture_01_floral_trench_coat.jpg', for example
	buynow: Buy Now URL if button is clicked
	module_exit: Index exited at, if index is present
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name

Video Playback Started:
	session_id: UID for overall session
	content_asset_id: Article ID of the video
	sound: sound (from 0-100)
	full_screen: boolean is fullscreen or not
	position: number representing current index position in seconds of the playhead
	total_length: total length of playback (including ads)
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name

Video Playback Completed:
	session_id: UID for overall session
	content_asset_id: Article ID of the video
	sound: sound (from 0-100)
	full_screen: boolean is fullscreen or not
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name

Video Content Started:
	session_id: UID for overall session
	asset_id: Article ID of the video
	title: Title of the video
	description: Description of video
	genre: Vertical of video
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name

Video Content Completed:
	session_id: UID for overall session
	asset_id: Article ID of the video
	title: Title of the video
	description: Description of video
	genre: Vertical of video
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name

Affiliate Clicked: Event fires whenever someone clicks an affiliate link (defined in CMS or by programmatic URL change)
	current_url: URL the user is currently on
	destination_url: Affiliate URL the user is directed to
	element: Essentially 'class' (ex. "vertical-image" or "vertical-title")
	image_id: Either the source or backend ID for the image, if applicable
	position: Article index (if in a slideshow, for example)
	article_title: The actual (in the CMS) title of the article
	title: Title as defined in CMS
	merchant: Merchant as defined in the CMS
	item: Item as defined in the CMS
	vendor: The partner vendor that is associated with the product (Skimlinks, BamX, Etc.)
	input_method: The way this link was ID'd as an affiliate link (CMS or programmatic)
	advertiser: If there is sponsorship behind the article, who is the advertiser
	article_type: The format of the article (List, Slideshow, Quiz, etc.)
	article_id: The unique ID of the article as defined by the backend
	author: The person who wrote the article
	category: The nav section of the article
	device: The device the user is using
	article_name: The actual (in the cms) title of the article
	construct: The platform the article is being served in (standard, amp, fbia)
	edition: The associated edition with the article
	pub_date: The publication date of the article
	sponsorship: The article 
	internal_experiment1: Our A/B testing name
	

