#### IN ACTION

[Portfolio](https://gatsby-strapi-portfolio-project.netlify.app/)

setup state value and fetch functionality
To display jobs on the ui, since the value state is initially set to zero, I can access the first job in the setJobs array, since it is not anymore an empty array, and grab the properties (company, duties, date, title) I need to display on the ui. This needs to happen after loading. Just after the loading, destructure those properties coming from job which is no longer an empty array, since jobs is fetched.
Note if the destructuring is not done after the loading, we will get an error, because before the loading, the array is empty, the array only gets filled with job data that can be destructured after the loading.
Only one job is displayed at this time because the value is hard coded to first index in the array. const [value, setValue] = useState(0)

Add buttons for all the job title we have on the array list. Once the button is clicked change the state value to 1, 2 etc accordingly. Display also updated state value.
Iterate over jobs, and for every job, display specific button.
Add onClick, clicking the button, adds the index which tells in the list where that job is. Also change the value once the button is clicked. The default value is zero, but as the button is clicked, the state in the value changes, and so the values for the properties.
on the button className, if the index matches the current state value, addd active-btn class.
