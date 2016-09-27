#!/usr/local/bin/node

var currentDate = new Date();
var time = currentDate.getHours();
var day = currentDate.getDay();
var season = currentDate.getMonth();

var timeScript;
var dayScript;
var seasonScript;

if (season < 2 || season > 10) {
    season = 1;  /*Winter*/
} else if (season > 1 && season < 5) {
    season = 2; /*Spring*/
} else if (season > 4 && season < 8) {
    season = 3; /*Summer*/
} else {
    season = 4; /*Spring*/
}

if (time < 10) {
    timeScript = "Time to get out of bed. You'll miss the best part of the day.";
} else if (time < 16) {
    timeScript = "Good Afternoon, whoever you are.";
} else if (time < 20) {
    timeScript = "Enjoying wasting your evening on YouTube? I know that's what you're doing.";
} else {
    timeScript = "Zzzzz-HEY I'M SLEEPIN' HERE! Ugh fine.";
}

if (day < 3) {
    dayScript = "Welcome to the beginning of the week, this one is never going to end. Really.";
} else if (day < 5) {
    dayScript = "I know you think we're nearing the end of the week, but we're not. You're wrong.";
} else {
    dayScript = "So it's the weekend. Enjoy pretending you have things to do.";
}

if (season === 3) {
    seasonScript = "It's summer, so hurry up and enjoy it before you remember you're an adult.";
    if (time > 4 && time < 10) {
        seasonScript += " Seriously. Get up. You're missing it.";
    }
} else if (season === 4) {
    seasonScript = "Oh, and don't Fall on your vacation! Er...uh, see you next time you trip!...just forget it.";
    if (time > 10 && time < 17) {
        seasonScript += " And don't forget to step outside and enjoy the weather on your lunch break...loser.";
    }
} else if (season === 1) {
    seasonScript = "Nothing to see here. It's still hot.";
    if (time > 16 && time < 22) {
        seasonScript += " And as it is both the evening and Winter...either put on a jacket or beware of heatstroke; I can't really help you here.";
    }
} else {
    seasonScript = "Spring means Spring Cleaning means it's time to empty my Trash Bin for the first time ever probably. Careful, I think there's something living in there.";
    if (time < 3 || time > 22) {
        seasonScript += " This is the Secret Picard.";
    }
}

if (season === 1 || season === 4) {
    seasonScript += " Also: be prepared for cold weather...or hot weather. SC stands for 'Seasons Can'tmakeuptheirminds'...yep.";
} else {
    seasonScript += " Also: beware of heatstroke.";
}

console.log(timeScript + " " + dayScript + " " + seasonScript);
