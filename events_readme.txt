Article Clicked: Event fires whenever someone clicks into an article, and they're already on the site.
	current_url: URL the user is currently on
	destination_url: URL the user is directed to
	element: Essentially 'class' (ex. "vertical-image" or "vertical-title")
	image_id: Either the source or backend ID for the image, if applicable
	position: Article index (if in a slideshow, for example)
	article_title: The actual (in the cms) title of the article

Article Shared: Event fires when one of the "share" buttons is clicked.
	current_url: URL the user is currently on
	action_type: Args will be Facebook, Pinterest, Text, Email, Print
	position: Article index (if in a slideshow, for example)
	location: 'surround_article' or 'incontent', for example
	element: 'pin_side' or 'facebook_stickynav', for example

Article Completed: Event fires when a user reaches the end of an article.
	current_url: URL the user is currently on

Slideshow Engaged: Event fires when a user clicks on any of the slideshow specific elements on the site.
	current_url: URL the user is currently on
	item_clicked: The URL of the article a user clicks (if applicable)
	slide_position: The furthest slide index the user reaches
	slide_exit: What slide index the user exits on

Navbar Clicked: Event fires when a user clicks on one of the navbar elements.
	current_url: URL the user is currently on
	element: 'food&recipes' or 'fashion&beauty', for example
	subelement: 'Home_01' or 'Travel_02', for example
	device: Args are Desktop/Mobile + OS

Footer Clicked: Event fires when a user clicks on any of the footer specific elements on the site.
	current_url: URL the user is currently on
	item_clicked: The URL of the article a user clicks (if applicable)
	element: 'privacy' or 'contests', for example
	device: Args are Desktop/Mobile + OS

EOP Clicked: Event fires when a user clicks on one of the EOP elements on the site.
	current_url: URL the user is currently on
	destination_url: URL the user is directed to
	element: 'zergnet_03_ARGS' or 'purewow_04_ARGS', for example
	position: Article index (if in a slideshow, for example)
	referral: Args will be Internal, Zergnet, PubExchange (etc.)
	module_type: 'desktop_partner_category' or 'eop_slider', for example
	article_title: Article a user clicks to (ex. 'h4 class="slider__hed"')

Right Rail Clicked:
	current_url: URL the user is currently on
	destination_url: URL the user is directed to
	element: 'zergnet_02', for example
	article_title: Article a user clicks to (in the hyperlink, as of 4/11/2017)

Newsletter Subscribed:
	current_url: URL the user is currently on
	user: Subscriber ID
	edition: Edition subscribed to
	source: How we acquired the email (Args BounceX or Internal)
	module: What module BounceX used or they subscribed internally from

Newsletter Unsubscribed:
	current_url: URL the user is currently on
	user: Subscriber ID
	edition: Edition subscribed to
	location: Where they unsubscribed from

Quiz Taken:
	current_url: URL the user is currently on
	questions_answered: Furthest question answered on the quiz
	result_viewed: Boolean result viewed yes/no
	quiz_retaken: Boolean quiz retaken or not
	quiz_shared: Where the quiz was shared to ('pin_quizresults_ARGS', for example)

Recipe Box Engaged:
	current_url: URL the user is currently on
	recipe_added: Recipe that's added
	recipe_removed: Recipe that's removed
	recipe_printed: If a user prints the recipe
	social_share: If/where a user shares on social, email, or text
	add_more_recipes: If a user clicks the add recipes box

Shop Module Engaged:
	current_url: URL the user is currently on
	module_position: Where the module itself appears
	item_clicked: '1_shopmodule_Topshop' or 'picture_01_floral_trench_coat.jpg', for example
	buynow: Buy Now URL if button is clicked
	module_exit: Index exited at, if index is present

Video Played:
	current_url: URL the user is currently on
	video_file: TODO Filename or link of video
	soundon: Boolean if sound is on or not
	video_title: Article title of the video

Video Completed:
	current_url: URL the user is currently on
	video_file: TODO Filename or link of video
	soundon: Boolean if sound is on or not
	video_title: Article title of the video

