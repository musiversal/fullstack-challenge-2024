=== Musiversal Booking App ===

Description:

We want to build an small application to reserve musicians on a daily basis, so we will show their available times and post a message in our website.

The designs and a bit of the interaction of what this DAW will include is in the following figma:

https://www.figma.com/file/EVSy3tsUIL4gNucNRAuoOk/Fullstack-Challenge-2024?type=design&node-id=0%3A1&mode=design&t=AS6436b73nxq4j5C-1

== Requirements and documentation:

The information about the musicians will be pull from our API and it will be fixed. The schedules will be fixed to the day the request is taking place. For instance, if today is 2024-01-01, the schedule dates will always be from that date, and if I run the same endpoint the day after, all dates will happen at the same time but the next day.

If the musician has enabled false, then it won't be displayed in the UI. On the time selection, past times will be shown blocked, same as times that have been already selected by another person. If the musician is "enabled false", then it won't display in the UI.

The API response will look like this:

```
  [
    {
      id: 1,
      name: 'Alicia Cooper',
      enabled: true,
      avatar: 'https://c8.alamy.com/compes/2r7a8r0/solvesborg-suecia-07-junio-de-2023-la-banda-ucraniana-de-heavy-metal-jinjer-realiza-un-concierto-en-vivo-durante-el-festival-de-musica-sueca-sweden-rock-festival-2023-en-solvesborg-aqui-la-vocalista-tatiana-shmailyuk-se-ve-en-vivo-en-el-escenario-credito-de-la-foto-gonzales-foto-terje-dokken-2r7a8r0.jpg',
      schedule: [
        "2024-01-01T12:15:00.000Z",
        "2024-01-01T19:15:00.000Z",
        "2024-01-01T20:15:00.000Z",
      ],
      "services": [
          "Guitar",
          "Bass"
      ]
    },
    {
      id: 1,
      name: 'Marino Manson',
      enabled: true,
      avatar: 'https://media.npr.org/assets/img/2015/02/09/marilyn-manson-credit-jiro-schneider_wide-74ef1df6aebb202ff9d45949cf10a7c07b812d13-s1400-c100.jpg',
      schedule: [
        "2024-01-01T13:15:00.000Z",
        "2024-01-01T14:20:00.000Z",
        "2024-01-01T22:15:00.000Z",
      ],
      "services": [
          "Vocals",
          "Drums"
      ]
    },
    {
      id: 1,
      name: 'Johnny Dept',
      enabled: true,
      avatar: 'https://media.vanityfair.com/photos/56c2a0c89895ef054035d775/master/pass/johnny-depp-hollywood-vampires-grammys.jpg',
      schedule: [
        "2024-01-01T15:15:00.000Z",
        "2024-01-01T19:15:00.000Z",
        "2024-01-01T23:15:00.000Z",
      ],
      "services": [
          "Sax",
          "Guitar"
      ]
    },
    {
      id: 1,
      name: 'Bruno Marz',
      enabled: true,
      avatar: 'https://los40.com/resizer/lxkeOmnI7JBxmVtm1yGVY9I5mfc=/1200x900/filters:format(jpg):quality(70)/cloudfront-eu-central-1.images.arcpublishing.com/prisaradiolos40/VA6MYF5ZAJMMFAHOIEDEA5TZHI.jpg',
      schedule: [
        "2024-01-01T12:15:00.000Z",
        "2024-01-01T19:15:00.000Z",
        "2024-01-01T20:15:00.000Z",
      ],
      "services": [
          "Vocals",
          "Bass"
      ]
    },
    {
      id: 1,
      name: 'Copernico Sanchez',
      enabled: false,
      avatar: 'https://i.blogs.es/50a1c5/t4yxpvu/1366_2000.jpeg',
      schedule: [
        "2024-01-01T12:15:00.000Z",
        "2024-01-01T19:15:00.000Z",
        "2024-01-01T20:15:00.000Z",
      ],
      "services": [
          "Guitar",
          "Bass"
      ]
    },

  ]
```

We don't have any restrictions on how to build your app, as long as you use ReactJS for the frontend and NodeJs for the backend. The information for each session needs to be stored in a database (we can use sqlite).

We need a README.md with launch/setup instructions, any technical choices you have made (which ones and why), additional features you added, known bugs or features that you would like to add to the app in the future.
Upload the code into a github/gitlab repo.

Some basic knowledge on unit tests is required. It doesn't mean you everything has to be tested, but we want to know you know your way around tests.
You can use any open source libraries as long as you specify why in the readme.
If you have any additional question please send us an email.

Happy coding!
