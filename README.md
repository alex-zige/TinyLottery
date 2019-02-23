# TinyLottery
A simple lottery application for Meetup.com.

## How to use
Meetup.com is a popular website to organize local community events. Sometimes it would be fun if there is a lucky draw for attendees at the end of the meetups. So I developed this tool to set a lottery.

### Getting attendees data
First, get the attendees data from meetup.com. Use Chrome and open your event page. On this page, you can find a section called `Attendees`. Click the link `Manage` to open the attendees page. The url is like this: https://www.meetup.com/{your-organization-name}/events/{event-id}/attendees/. You can see all the attendees here.

Press `F12` to enable developer tools and navigate to `Network` tab. Then press `F5` to refresh the page. In the `Network` window, you can find requests about attendees data. Find the correct one. Usually, it should start with `https://www.meetup.com/mu_api/urlname/events/eventId/attendees?queries=%28endpoint%3A{you-organization-name}...`. Click `Response` tab, now you can get all attendees data. Copy the content and save it as a json file called `attendees.json`;

### Clone and build the project on your laptop
It would be better if I integrate the meetup login system and publish it as a website. But it is also very easy to use it on your laptop. Clone the project and navigate to the `tiny-lottery` folder. Copy the `attendees.json` file and paste it into the `assets` folder. Then use the command below to run it:

```bash
ng run --open
```

That's it!

## Contact me
yan_xiaodi{at}hotmail.com