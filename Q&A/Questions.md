Q&A
===
###Questions for Studiocracy
**Response by Chris Robles 07/14/15 via Slack**
  * What is the preferred language to be used for creating an analytics fact table?
    - We use postgreSQL for our db's
  * For the current tables shown in your db schema is there a meta data file describing the fields?
    - As for a file describing all the fields in our schema I would have to check. We are planning on doing some cleanup on our db so we would have to make sure to update you guys.
  * Do you currently have content within your tables that we could have access to for testing?
    - For content in the tables we're using generated dummy content created by the seeds.rb file under db folder, we can add some additional content to it so that it better covers all the fields.
  * Is there a preferred color pallet for visuals?
    - As far as a color pallet, I can talk to our designers and see if they have anything in mind.
  * In regards to the location of the dashboards on which page will it be displayed?
    - The analytics table will be in an admin page. But we also like the idea of having one accessible to users so that they can see statistics on their content.
  * Show mock-up of the artist dashboard for initial suggestions.
    - Generally the mock up looks good, it's what we're looking for.
  * Is Tableau the preferred software for analytics?
    - Tableau looks like it'll work great.
  * What are the requirements for admin dashboard?
   - The purpose of the dashboards is for us to track statistics of our user base, and for artist to track statistics on their content. I'll bring it up at tomorrow's meeting and talk to our designers to discuss specifics on how it should look, and we'll figure out exactly what statistics we'd be looking to track.

**Response by Julian De Ocampo 07/14/15 via GitHub**
  * What is the preferred language to be used for creating an analytics fact table?
    - SQL, preferably using PostgreSQL if you can pick databases.
    - Not sure how Tableau works but I'm guessing it uses some sort of JavaScript framework to construct the visualizations. I'd definitely prefer interactive JS visualizations (there are a lot of frameworks out there you can choose from) over a program that just spits out static images.
  * For the current tables shown in your db schema is there a meta data file describing the fields?
    - Yes. studiocracy-public => app => db => schema.rb
    - Table may be trimmed or edited with time, so I would pull from the main repo or check it frequently.
  * Do you currently have content within your tables that we could have access to for testing?
    - Sort of. In Rails, you connect to a database and you can populate it with test data using rake db:seed. This will generate test data based on a file called seed.db under the db folder in app. However, the seed.rb file is a little rough right now and might need some work on both of our ends to get into shape for our goals. The database itself might also need to have additions or removals.
  * Is there a preferred color pallet for visuals?
    - Refer to our style guide: https://docs.google.com/document/d/1BOQp0eG4K54nQShN7ZFKjAPZe7r9svvCICfNmQQJndI/edit?usp=sharing
  * In regards to the location of the dashboards on which page will it be displayed?
    - Users who log in will be able to view their dashboard and see how their studio is doing. They can also elect to share and place any of the visualizations on their public portfolio page.
  * Show mock-up of the artist dashboard for initial suggestions.
    - Mockup for the visualizations looks good. I'll speak with our designers to see if we can get you a proposed version of the dashboard. For now focus on the data analytics and visualizations rather than layout.
  * Is Tableau the preferred software for analytics?
    - Maybe. I need you to run cost estimates. Because our codebase is an open source project and our company is a startup, we don't want to blow thousands of dollars on an annual license on software to power bonus features before we've launched. It would be better to look into open source data visualization frameworks
  * What are the requirements for admin dashboard?
   - Chris's answer is fine. Artists need to be able to see a dashboard with visualizations that they can flip through to see how their personal engagement, reputation, views, and sales are going. Some of these features, like a reputation or karma system, are not yet implemented and need to be designed with your help.
