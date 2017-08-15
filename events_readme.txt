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

(Social) Article Shared: Event fires when one of the "share" buttons is clicked.
	current_url: URL the user is currently on
	action_type: Args will be Facebook, Pinterest, Text, Email, Print
	position: Article index (if in a slideshow, for example)
	location: 'surround_article' or 'incontent', for example
	element: 'side' or 'stickynav', for example

Article Completed: Event fires when a user reaches the end of an article.
	current_url: URL the user is currently on

Slideshow Engaged: Event fires when a user clicks on any of the slideshow specific elements on the site.
	current_url: URL the user is currently on
	item_clicked: The URL of the article a user clicks (if applicable)
	slide_position: The furthest slide index the user reaches
	slide_exit: What slide index the user exits on

Navbar Clicked: Event fires when a user clicks on one of the navbar elements.
	current_url: URL the user is currently on
	location: Explicitly either the "top" nav or the "side" nav
	element: fashion/beauty/recipes/home/family/how-tos OR lifestyle/trending/videos/cities
	subelement: null if location == top; child to element if location == side
	device: Args are Desktop/Mobile + OS

Footer Clicked: Event fires when a user clicks on any of the footer specific elements on the site.
	current_url: URL the user is currently on
	item_clicked: The URL of the article a user clicks (if applicable)
	element: 'privacy' or 'contests', for example
	device: Args are Desktop/Mobile + OS

(Referral) EOP Clicked: Event fires when a user clicks on one of the EOP elements on the site.
	current_url: URL the user is currently on
	destination_url: URL the user is directed to
	element: 'zergnet_03_ARGS' or 'purewow_04_ARGS', for example
	position: Article index (if in a slideshow, for example)
	—-referral: Args will be Internal, Zergnet, PubExchange (etc.)
	module_type: 'desktop_partner_category' or 'eop_slider', for example
	article_title: Article a user clicks to (ex. 'h4 class="slider__hed"')

Right Rail Clicked:
	current_url: URL the user is currently on
	destination_url: URL the user is directed to
	element: 'zergnet_02', for example
	article_title: Article a user clicks to (in the hyperlink, as of 4/11/2017)

Quiz Taken:
	current_url: URL the user is currently on
	questions_answered: Furthest question answered on the quiz
	result_viewed: Actual output of the result, if viewed
	quiz_retaken: Boolean quiz retaken or not
	quiz_shared: Where the quiz was shared to ('pin_quizresults_ARGS', for example)
	back_button_clicked: If the back button on the quiz (not in the browser) was clicked
	answers_given: Specific answers chosen on the quiz, returned as a demlimited string in one "cell"
	
Pinterest Quiz Taken:
	current_url: URL the user is currently on
	questions_answered: Furthest question answered on the quiz
	pin_viewed: If the user went to Pinterest to see their pin; Bool
	quiz_retaken: Boolean quiz retaken or not
	quiz_shared: Where the quiz was shared to ('pin_quizresults_ARGS', for example)
	back_button_clicked: If the back button on the quiz (not in the browser) was clicked
	answers_given: Specific answers chosen on the quiz, returned as a demlimited string in one "cell"

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

Video Playback Started:
	session_id: UID for overall session
	content_asset_id: Article ID of the video
	sound: sound (from 0-100)
	full_screen: boolean is fullscreen or not
	position: number representing current index position in seconds of the playhead
	total_length: total length of playback (including ads)

Video Playback Completed:
	session_id: UID for overall session
	content_asset_id: Article ID of the video
	sound: sound (from 0-100)
	full_screen: boolean is fullscreen or not

Video Content Started:
	session_id: UID for overall session
	asset_id: Article ID of the video
	title: Title of the video
	description: Description of video
	genre: Vertical of video

Video Content Completed:
	session_id: UID for overall session
	asset_id: Article ID of the video
	title: Title of the video
	description: Description of video
	genre: Vertical of video

