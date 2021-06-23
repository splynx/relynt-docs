Administrators can link Relynt to their Google accounts to sync tasks assigned (and scheduled) to them onto their Google calendars.

![Scheduling](scheduling.png)

To connect a Google account, click on the **Connect Google account** button and follow the steps.

After clicking on the "Add Google account" button, the following window will appear:

![Authorization](authorize.png)

* 1. Click on the Google authorize link to sign in. You will be redirected to the Google sign in page. Follow the instructions and allow using the Relynt calendar into the Google account.

* 2.You will then receive a code which you need to enter into the field provided to connect the Google calendar to Relynt. Simply copy this code into the provided field

* 3. Click on *connect Google account* to complete the process:

![Google authorized](linked_google_acccount.png)

To sync Relynt tasks to the connected Google calendar, it is necessary to add a paired calendar. This allows the Relynt calendar of the administrator to sync items into the Google calendar. Simply click on the + add paired calendar button to add a paired calendar:

![add admin's calendar](add_admin_calendar.png)

Once this is done, let's assign a task to this admin:

![Assigned to admin task](task_assigned_to_admin.png)

Now the admin will be able to see this task directly on their Google calendar:

![task for admin under google calendar](googlee_assigned_to_admin.png)

Let's imagine a scenario when you add a [scheduling team](configuration/scheduling/teams/teams.md) named "Technicians" where a current admin is a member of this team. You assigned a task to the team "Technicians":

![task_assigned_to_team](task_assigned_to_team.png)

and even if the admin is a member of the team, the task was not synced to Google calendar:

![empty Google calendar](empty_google_calendar.png)

The reason for this is that you did not pair the calendar of this team. Let's apply this:

![pair team calendar](add_team_calendar.png)

once this done, you can check your Google calendar:

![google_assigned_to_team](google_assigned_to_team.png)

**Conclusion**: if an admin wants to sync tasks that are assigned directly to him and tasks that are assigned to a team(where this admin is a member), it's necessary to pair the personal calendar and the team calendar:

![final setup](final_setup.png)

Note that if the admin is a member of few teams, each calendar of this team needs to be paired here to sync tasks assigned to these teams.
