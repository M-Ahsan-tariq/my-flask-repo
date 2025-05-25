<pre>
<h1>Project Title: "Web Development Project with Flask"
Website name: FitZone</h1>
<h3>Purpose of Fit Zone Website:</h3>
• Fitness Hub: Dedicated to health & fitness enthusiasts
• Provide workout plans & fitness services
• Showcase exercise gallery & transformations
• Enable user accounts (login/register)
• Offer contact for fitness inquiries
<h3>Website Structure:</h3>
• Home-Banner, intro, navigation
• About- Mission, trainers, gym photos
* Membership-
<h1>Home Page</h1>
<h3>Frontend:</h3>
The website starts with the Home Page, which is the index.html file. It contains a welcoming message for FitZone users and offers a variety of navigation options that link to other pages such as About Us and Membership.
•The page is built using HTML and styled using CSS.
•Text and images are placed using standard HTML tags.
•Navigation is created using anchor (<a>) tags to link between different pages.
•Images are added using the <img> tag.
<h3>Key HTML Functions:</h3>
&lt;a href="page.html"&gt;Link&lt;/a&gt; → Used to link to other pages like About or Membership
&lt;img src="image.jpg"&gt; → Used to display images on the homepage
<h3>Backend (Flask):</h3>
In the backend, Flask serves the Home Page using a route defined in app.py. This route tells Flask to render the index.html template when the root URL is accessed.
<h3>python:</h3>
@app.route('/')
def home():
    return render_template('index.html')
  
<h1>About Us Page:</h1>
<h3>Frontend:</h3>
The About Us Page provides the background and history of FitZone Gym, as well as more navigation options for accessing other sections of the website.
•It is also built with HTML and styled using CSS.
•Contains descriptive text placed within the &lt;body&gt;
•Navigation to other pages is handled using anchor tags.
•Images are added similarly using the &lt;img&gt; tag.
<h3>Key HTML Functions:</h3>
&lt;a href="index.html"&gt;Home&lt;/a&gt; → Links back to Home Page
&lt;img src="gym.jpg"&gt; → Displays an image on the About Us page
<h3>Backend (Flask):</h3>
The About Us Page is rendered through a dedicated Flask route in app.py. When the user visits /about, Flask loads the about.html template.
<h3>python:</h3>
@app.route('/about')
def about():
    return render_template('about.html')
<h1>Membership Page:</h1>
<h3>Frontend:</h3>
The Membership Page presents details about FitZone's various membership plans. It includes pricing, benefits, and a form for user sign-up or inquiries.
•Structured using HTML and styled with CSS.
•The form elements can collect data like name, email, membership type, etc.
•Navigation and images are handled using the same methods as in previous pages.
<h3>Key HTML Functions:</h3>
&lt;a href="about.html"&gt;About Us&lt;/a&gt; → Allows users to navigate back.
<h3>Backend (Flask):</h3>
Flask handles the rendering and optional form processing on the Membership Page. A route is set up to load the page when the /membership URL is visited.
<h3>python</h3>
@app.route('/membership')
def membership():
    return render_template('membership.html')
</pre>
