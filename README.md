# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)

# Predicted User Scenarios

Feature 2: Show/Hide an event’s details
	
As a user,
	I should be able to show or hide and event’s details,
	So that I can see or not see a certain event’s details

	Scenario 1: An event element is collapsed by default
	Given user has not clicked on an event element
	When the user opens the app
Then the event element should be collapsed

Scenario 2: User can expand an event to see its details
Given a user is looking for event information
When the user opens the app
Then they should be able to toggle the event to show details

Scenario 3: User can collapse an event to hide its details
Given a user wants to hide event details
When they have them toggled
Then they should be able to collapse the event details

Feature 3: Specify number of events
	As a user,
	I should be able to specify a number of events,
	So that I can see a specific number of events

	Scenario 1: When user hasn’t specified a number, 32 is the default number
	Given a user has not specified the number of events they want shown
	When they are searching events
	Then the default number should be 32
	
	Scenario 2: User can change the number of events they want to see
	Given a user wants to see more or less than 32 events
	When they are searching events
	Then they should be able to change the number of events they can see
	

Feature 4: Use the app when offline
	As a user,
	I should be able to use the app offline,
	So that I can use the app while offline

	

Scenario 1: Show cached data when there’s no internet connection
	Given a user wants to use the app
	When they are offline
	Then they should be able to see cached data

Scenario 2: Show error when user changes the settings (city, time range)
	Given a user tries to change settings (city, time range)
	When they are offline
	Then the app should show an error

Feature 5: Data visualization
	As a user,
	I should be able to see a chart with the number of upcoming events,
	So I can better read the data

Scenario 1: Show a chart with the number of upcoming events in each city
	Given a user wants to see the number of events
	When they are searching by city
	Then they should see a chart that lists this info
	

