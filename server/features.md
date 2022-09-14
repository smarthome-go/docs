## Dashboard
The dashboard aggregates the system's data and metrics and shows it in a human-friendly way.
Once you are logged in successfully, you will be redirected to the dashboard.

### Power Usage
This graph shows the historic power usage of the last 24 hours.
The x-axis spans over time whilst the y-axis shows the power usage at any given point in time.

### Quick Actions
If you enable *Quick Actions* for any of your Homescript, it will be considered as an action which you can run quickly.
Those special scripts will show up in the *Quick Actions* box and will give you the opportunity to run predefined tasks quickly.
Once you run an action, the results will be presented as a popup.

### Weather
This box shows the current whether in your location.
In order to use the weather box, a valid *OpenWeatherMap* API token is required.

### Schedules & Automations
Any upcoming automations will be shown on the left-hand side whilst any pending schedule will be shown on the right-hand side.

### Reminders
All your reminders will be shown in this box, allowing you to get a grasp of your pending tasks.
You can also use the checkbox on the right of each reminder to mark it as *complete*.

## Rooms
Shows all rooms and their contents, such as switches and cameras.
If you are in possession of the *manage rooms* permission, the rooms page can be used in order to manage rooms.
Switches and cameras can be viewed, added, modified and deleted.

If you are not in possession of this permission, the rooms page can be used to interact with switches and view camera feeds,
Which switches and cameras are shown still depends on the `camera` and `switch` `permissions` of the target user.

## Reminders
Just like a to-do app, just inside Smarthome so that forgetting things becomes much harder.
The inputs on the right can be used to create a new reminder.
The edit icon on every reminder can be used to edit that reminder.
When a task is completed, the check mark on the top right of each reminder can be used to mark it as completed.

## Scheduler
The scheduler page is to be used when planning an action which will only run once, such as waking up earlier.
Each schedule is executed at a point in time which is set when creating a new schedule.
When a schedule is executed, it is removed from the page so that it only runs once.

What happens when the schedule executes depends on your needs.
If the action is already defined, you can just choose a Homescript from the list (*but make sure selection is checked on the desired Homescript*).
Otherwise, if one or more switches should change their power state, the *switches* tab is to be used.
Otherwise, the *Homescrip Codet* tab allows you to write custom Homescript code as a schedule's target.

## Automations
Automations are similar to schedules with the main difference being that automations run multiple times.
This makes automations feasible for setting a complete automated workflow which can be customized to fit your needs.
However, automations only accept a selected Homescript as their target.
To allow for more precise control over the automations, weekdays and sunset / sunrise settings can be customized when setting-up an automation. 

## Homescript
Homescript is Smarthome's own scripting language which allows users to set up their own routines and functions.
Every Homescript is identified by its id and holds metadata, for example a name, or it's code.
Additionally, arguments can be set up in order to pass values or decisions to the Homescript when it is executed.
For example, consider a script which turns a switch off, then on.
The switch could be passed in as an argument, thus making this script universal and more practical. 
A Homescript can either be executed or linted, a process which checks for possible errors in the code and shows them to you.

## Homescript Editor
If you press the *code* button when editing a Homescript, you enter the Homescript IDE / editor.
This page allows you to edit your Homescript code easily.
On the right, there is a terminal which would show any execution or linting outputs.
On the left, a text editor allows you to write your Homescript code.
When you type, the code is automatically linted and possible issues are displayed in the editor.

## Profile
The place where you can customize your settings and change your avatar.
You can also choose to change your password or delete your user entirely.
If you disable schedules and automations here, your user's schedules and automations will not run with any effect, thus making this setting useful for traveling.

## Users
The user management page allows you to view, add, edit and delete Smarthome users.
You can also specify a user's permission set which increases the systems' security.

## System
Settings on this page effect the entire Smarthome server.
Here, you must configure your hardware devices so that Smarthome can interact with the real world.
Furthermore, you can set up your *OpenWeatherMap* API key in here in order to allow Smarthome users to obtain weather data.
Lastly, you can even export or import the entire system settings so that a Smarthome setup is easily reproducible.

