#### IN ACTION

[Portfolio](https://gatsby-strapi-portfolio-project.netlify.app/)

setup state value and fetch functionality
To display jobs on the ui, since the value state is initially set to zero, I can access the first job in the setJobs array, since it is not anymore an empty array, and grab the properties (company, duties, date, title) I need to display on the ui. This needs to happen after loading. Just after the loading, destructure those properties coming from job which is no longer an empty array, since jobs is fetched.
Note if the destructuring is not done after the loading, we will get an error, because before the loading, the array is empty, the array only gets filled with job data that can be destructured after the loading.
Only one job is displayed at this time because the value is hard coded to first index in the array. const [value, setValue] = useState(0)
