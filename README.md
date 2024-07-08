# FlavourSafari
FlavourSafari is a recipe finder website👩‍🍳

sometimes it’s a real hassle trying to find the perfect recipe online. With our FlavourSafari websiter, we are going to make that search a piece of cake! Users can say goodbye to endless scrolling and confusing websites. Our webapp will be like a treasure chest, making it super easy to discover delicious dishes based on what they’re craving or the ingredients they have on hand. The website will operate by fetching recipe data from a food API, displaying it in a user-friendly interface and providing a seamless experience for discovering and organizing recipes. 

 
TEAM 
Our team is a blend of creativity and tech-savviness, cooking up a delicious app that will revolutionize how people discover recipes 
•	Wandia Muhoro – Dancer, an electrical engineer and an awesome code wizard 

•	Monicah Mugure – Baker, crocheter  and a top-notch tech guru 
 
TECHNOLOGIES
	
Languages 

• HTML and CSS for structuring the content of the app and making it virtually appealing by styling it.

•JavaScript- add  front-end interactivity, dynamic functionality and will be used for back-end server logic.

Platforms 
• GitHub: For managing and collaboration. 

Books/Resources 
• Mozilla Developer Network: For HTML, CSS, and JavaScript documentation.

Technology Choice Analysis 

-Fetch API over Axios because it is Native to modern browsers and there is no need for additional libraries.
 
CHALLENGE 

Our portfolio project is Intended to  address the challenge of meal planning and recipe 
discovery based on available ingredients. Often, individuals struggle with deciding what 
to cook with the ingredients they have at home. This can lead to wasted food, repeated meals, or unhealthy eating habits. The app provides a simple solution by allowing users to input available ingredients and receive a list of recipes that they can make. 

What the Portfolio Project Will Not Solve
1. Personalized Dietary Preference:While the app can suggest recipes based on ingredients, it may not fully account for specific dietary preferences.
2. Cooking Skills: The webapp assumes users have basic cooking knowledge and skills. It will 
not provide in-depth cooking tutorials or guidance for complete beginners. 
 
Language Support: Initially, the webapp may be available only in English. Expanding 
language support can make it more accessible to non-English speaking users around the world. 
By addressing these considerations, our recipe finder app aims to provide a valuable 
tool for a wide range of users globally, helping them to discover new recipes, reduce food waste, and simplify meal planning. 
 
RISKS
Technical Risks 
1. API Reliability and Changes

• Potential Impact: The app relies on a third-party food API for fetching recipe data. If 
the API experiences downtime, changes in endpoints, or rate limits, it could disrupt the 
app’s functionality. 
- Safeguards: 
•	Implement error handling to manage API failures and provide users with appropriate messages.
•	Use caching strategies to store frequently accessed data. 
•	Monitor API usage and set up alerts for any anomalies. 
2. Data Privacy and Security 
• Potential Impact: Handling user data, such as ingredient inputs or saved recipes, poses privacy and security risks. Data breaches or leaks could damage user trust and result in legal consequences. 
- Safeguards: 
•	Ensure secure communication using HTTPS. 
•	Implement proper data encryption for any stored user data. 
•	Follow best practices for authentication and authorization. 
•	Regularly update dependencies to patch security vulnerabilities. 
3. Cross-Browser Compatibility	 
-Potential Impact: The app may not function correctly on all browsers, leading to a poor user experience for some users. 
- Safeguards: 
•	Test the application on multiple browsers and devices to ensure compatibility. Use modern, widely supported web technologies and polyfills where necessary. 
Non-Technical Risks 
1. User Adoption and Engagement	 
• Potential Impact: If the app does not attract enough users or fails to engage them, it 
could lead to low usage and eventual abandonment. 
-Strategies: 
•	Conduct market research to understand user needs and preferences.
•	Implement user feedback mechanisms to continuously improve the app. 
•	Use marketing strategies such as social media promotion, SEO, and partnerships to increase visibility. 
2. Legal and Compliance Issues 
•Potential Impact: Non-compliance with data protection regulations (e.g., GDPR, CCPA) could result in legal penalties and damage to reputation. 
-Strategies: 
•	Ensure compliance with relevant data protection laws by implementing necessary policies and practices. 
•	Regularly review and update the app’s privacy policy. 
•	Seek legal advice to stay informed about regulatory changes. 
3. User Trust and Satisfaction 
•Potential Impact: Negative user experiences or data privacy concerns could erode trust and satisfaction, leading to negative reviews and loss of users. 
-Strategies: 
•	Prioritize user-centric design and development. 
•	Provide transparent communication about data usage and privacy. Implement robust customer support to address user issues promptly. 
By addressing these technical and non-technical risks with appropriate safeguards and 
strategies, the Recipe Finder app aims to provide a reliable, secure, and user-friendly 
experience, fostering growth and user satisfaction. 

INFRASTRUCTURE.
Branching and Merging Strategy
GitHub Flow
To maintain a structured and efficient workflow, we will use the GitHub Flow branching strategy. Here’s a detailed process for branching and merging:
1. Main Branch: The main branch will be the production-ready branch, containing the
latest stable code.
2. Feature Branches: For each new feature or bug fix, create a new branch from main.
Name the branch descriptively, such as feature/add-search-functionality or fix/button-style       	.
3. Developing Features  :
                            	
•Work on the feature or fix in your feature branch.
•Regularly commit your changes with clear and concise messages.
4. Pull Requests:
•Once the feature is complete and tested locally, open a pull request (PR) to merge the feature branch into main.
•Ensure that the PR description is detailed, including what the feature/fix entails and any relevant screenshots or notes.
5.Code Review:
•Team members review the PR for code quality, functionality, and potential issues.
•Address any feedback and make necessary changes.
6. Merging:
•Once approved, the PR is merged into main.
•Optionally, use “Squash and Merge” to keep a clean commit history.
This strategy ensures that main always contains stable and deployable code, while
feature branches allow for isolated development and thorough review before merging.
Data Population Strategy
Using the Spoonacular API       	
1. Fetching Data :
•Use Fetch API to make HTTP requests to the Spoonacular API to fetch recipes based on user inputs.
•Implement a server-side route (/Api/recipes) that handles these requests and sends the data to the frontend.
2. Caching:
•Implement caching mechanisms to store frequently accessed data and reduce API call frequency.
•Use an in-memory cache like Redis if necessary for performance improvement.
3. Seed Data for Development:
•Create a set of sample data for local development and testing to simulate API responses.
•This ensures that development can proceed without hitting the API rate limits.
Testing Tools and Automation
1. Unit Testing:
                            	
• Use Jest for unit testing JavaScript code
• Write tests for critical functions, API calls, and data handling processes.
2. Integration Testing:
* Use a tool like Supertest alongside Jest to test API endpoints and ensure that different parts of the application work together as expected..
4. Continuous Integration (CI) 	:
•Set up GitHub Actions to run automated tests on each push and pull request.
•Configure CI to run the test suite, ensuring that only code that passes all tests is merged into main.
5. Linting and Code Quality:
•Use ESLint to enforce coding standards and catch potential issues early.
•Integrate Prettier for consistent code formatting.
•Set up pre-commit hooks using Husky to run linting and formatting checks before code
is committed.
 
EXISTING SOLUTIONS.
Existing Solutions
Similar Products or Solutions
1. Allrecipes  	
Similarities:
•Allows users to search for recipes based on ingredients.
• Provides detailed recipes with instructions, ratings, and reviews.
Differences:
•Allrecipes is a comprehensive platform with a vast user community and additional
features like meal planning and shopping lists.
•The user interface is more complex, targeting a wide range of culinary needs.
2. Yummly
Similarities:
•Ingredient-based recipe search functionality.
• Personalized recipe recommendations based on user preferences and dietary
restrictions.
Differences:
•Yummly has a more advanced recommendation engine powered by machine learning.
•Includes features like meal planning, grocery delivery integration, and smart appliance connectivity. 
Reimplementing a Proven Solution Class of Solution: Recipe Finder Apps
Chosen Specification: Ingredient-Based Recipe Search with User-Friendly Interface
Rationale for Reimplementation:           	
* Simplicity and Focus	: Many existing solutions offer a wide range of features, which can be overwhelming for users looking for a simple, straightforward tool to find recipes based on ingredients they have. Our solution focuses on simplicity and usability, making it easy for users to quickly find recipes without navigating through numerous additional features.
* Customization and Control: By developing our own solution, we have full control over the user experience, design, and functionality. This allows us to tailor the app to specific user needs and preferences, which might not be possible with off-the-shelf solutions.
* Educational Opportunity: Reimplementing this solution provides an educational experience for the development team, allowing us to learn and apply various technologies and best practices in web development, API integration, and user interface design.
Proven Solutions:        	
1. Allrecipes Model:
•Strengths: Comprehensive features, large user base, and community-generated content.
•Weaknesses: Complexity and potential for feature overload for users looking for simple recipe searches.
2. Yummly Model:
•Strengths: Advanced personalization and recommendation engine, integration with other services.
•Weaknesses: May require significant resources and expertise in machine learning to replicate the recommendation system.
Chosen Specification Justification:       	
*User-Focused Simplicity: The primary goal is to create an easy-to-use tool that helps users find recipes quickly based on their available ingredients. By focusing on this core functionality, we can ensure a seamless and satisfying user experience.
*Flexibility and Adaptability: Developing our own solution allows us to adapt and expand the app based on user feedback and changing needs. We can add features incrementally without the constraints of an existing platform.
*Educational and Developmental Benefits: The reimplementation process provides valuable learning experiences for the development team, enhancing skills in web development, API integration, and user experience design.
By understanding and leveraging the strengths of existing solutions while addressing their weaknesses, we aim to create a streamlined, user-centric recipe finder app that offers a unique value proposition in the market.


Architecture


![FlavourQuest_System_Architecture_(light) drawio 1](https://github.com/MonicahKoina/FlavorQuest/assets/145972252/cf5c4ce9-3483-4441-8f24-96e2745f3013)



APIs and Methods
API Routes for Recipe Finder Web App
1. Search Recipes
Endpoint: /api/recipes/search
Methods:
GET: Returns an array of recipes that match the search query.
POST: Takes search parameters and returns matching recipes.
Example:
GET /api/recipes/search?query=pasta: Searches for recipes containing "pasta".
POST /api/recipes/search:
json
{ "query": "pasta", "number": 10 }
2. Get Recipe Details
Endpoint: /api/recipes/:id
Method: GET
Description: Returns detailed information about a specific recipe.
Example:
GET /api/recipes/12345: Gets details for recipe with ID 12345.
3. Get Recipe Instructions
Endpoint: /api/recipes/:id/instructions
Method: GET
Description: Returns the step-by-step instructions for a specific recipe.
Example:
GET /api/recipes/12345/instructions: Gets instructions for recipe with ID 12345.
I’ll be using the spoonacular API
Spoonacular API
GET /recipes/complexSearch
Description: Search for recipes using a wide variety of possible parameters.
Endpoint: https://api.spoonacular.com/recipes/complexSearch
Parameters:
query: The search query (e.g., "pasta").
diet: Filter recipes by diet type (e.g., "vegetarian").
cuisine: Filter recipes by cuisine (e.g., "Italian").
intolerances: Filter recipes by intolerances (e.g., "gluten").
number: Number of results to return (default is 10).
Example: GET /recipes/complexSearch?query=pasta&diet=vegetarian&number=10
GET /recipes/{id}/information
Description: Get information about a specific recipe.
Endpoint: https://api.spoonacular.com/recipes/{id}/information
Parameters:
includeNutrition: Whether to include nutrition information in the response.
Example: GET /recipes/12345/information?includeNutrition=true
POST /food/ingredients/search
Description: Search for ingredients using a wide variety of possible parameters.
Endpoint: https://api.spoonacular.com/food/ingredients/search
Parameters:
query: The search query (e.g., "apple").
number: Number of results to return (default is 10).
User Stories
1. As a user, I want to save my favorite recipes so that I can easily find them later. I want something like a special notebook where I can write down my favorite recipes.
2.As a user, I want to view detailed instructions for a recipe so that I can follow along while cooking.When i click on a recipe, it shows me all the details like ingredients, how much of each ingredient i need, and the steps to cook the dish.
3.As a user, I want to add a review to a recipe so that I can share my experience with others.I want to tell everyone how yummy it was or if there were any problems.

Mockups


