# Notification-Drawer

## Usage

```JS
import Notifications from './notificationDrawer'

let notif = new Notifications('topright', 'notifications')

notif.sendNotification(
    'success',
    {
        title: 'Success!',
        body: 'The action ended without any problems :D'
    }, 2000
)
```

### constructor(Orientation, Id)

Initializes a new Notification Drawer object that'll display notifications in the corner of the screen specified as **Orientation**.  
The div that'll contain the notifications will have a class "notification-drawer-**Id**"

When more than one Notification Drawer is initialized, the Ids must be different.

### sendNotification(Type, {Title, Body}, On-screen time (ms))

sends a notification of a given type on the screen, this notification will have a title and a body, and will be displayed for a given amount of time

possible values for **Type**: 'success', 'info', 'warning', 'error'
