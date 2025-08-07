# FootballBooking

This project was generated using [Angular CLI](https://github.com/angular/angular-cli) version 20.0.5.

## Project Structure
 └── frontend
    ├── .editorconfig
    ├── .gitignore
    ├── .vscode
        ├── extensions.json
        ├── launch.json
        └── tasks.json
    ├── Dockerfile
    ├── README.md
    ├── angular.json
    ├── docker-compose.yml
    ├── package-lock.json
    ├── package.json
    ├── proxy.conf.json
    ├── public
        ├── 3139256.jpg
        ├── 360_F_868510427_vsvN67LV1zSmLMyXMOFG05tRCmTAj1xL.jpg
        ├── 5.jpg
        ├── Awesome-Camp-Nou-Background.jpg
        ├── FCB-OFICIAL-1er-masc-2425-051_ALTA_LOGO.jpg
        ├── LOGIN.png
        ├── Mini Estadi.webp
        ├── barcelona football team group.jpg
        ├── campnou-2-2.jpg
        ├── favicon.ico
        ├── field icon.png
        ├── field.png
        ├── il_570xN.4352455753_jinn.avif
        ├── logo.png
        ├── match-schedule.webp
        ├── notification bell icon.png
        ├── photo-1585170236738-aadfce97f025.jpeg
        └── team management.jpg
    ├── src
        ├── app
        │   ├── app.config.ts
        │   ├── app.css
        │   ├── app.html
        │   ├── app.routes.ts
        │   ├── app.spec.ts
        │   ├── app.ts
        │   ├── core
        │   │   ├── enums
        │   │   │   ├── place-type.enum.ts
        │   │   │   └── user-role.ts
        │   │   ├── guards
        │   │   │   └── auth-guard.ts
        │   │   ├── interceptors
        │   │   │   ├── auth.interceptor.ts
        │   │   │   ├── error.interceptor.ts
        │   │   │   └── token-interceptor.ts
        │   │   ├── models
        │   │   │   ├── ierror-code.model.ts
        │   │   │   ├── iplace.model.ts
        │   │   │   ├── iteam-member.model.ts
        │   │   │   └── iuser.model.ts
        │   │   ├── services
        │   │   │   ├── auth.service.ts
        │   │   │   ├── booking.service.ts
        │   │   │   ├── error-handler.service.ts
        │   │   │   ├── error-mapping.service.ts
        │   │   │   ├── match-participant.service.ts
        │   │   │   ├── notification.service.ts
        │   │   │   ├── place.service.ts
        │   │   │   ├── team-member.service.ts
        │   │   │   ├── team.service.ts
        │   │   │   ├── user.service.ts
        │   │   │   └── websocket.service.ts
        │   │   └── utils
        │   │   │   ├── error-utils.ts
        │   │   │   └── utils.ts
        │   ├── features
        │   │   ├── auth
        │   │   │   ├── login
        │   │   │   │   ├── login.css
        │   │   │   │   ├── login.html
        │   │   │   │   └── login.ts
        │   │   │   └── register
        │   │   │   │   ├── register.css
        │   │   │   │   ├── register.html
        │   │   │   │   └── register.ts
        │   │   ├── bookings
        │   │   │   ├── admin-booking-management
        │   │   │   │   ├── admin-booking-management.css
        │   │   │   │   ├── admin-booking-management.html
        │   │   │   │   └── admin-booking-management.ts
        │   │   │   ├── booking-details
        │   │   │   │   ├── booking-details.css
        │   │   │   │   ├── booking-details.html
        │   │   │   │   └── booking-details.ts
        │   │   │   ├── booking-form
        │   │   │   │   ├── booking-form.css
        │   │   │   │   ├── booking-form.html
        │   │   │   │   └── booking-form.ts
        │   │   │   ├── booking-list
        │   │   │   │   ├── booking-list.css
        │   │   │   │   ├── booking-list.html
        │   │   │   │   └── booking-list.ts
        │   │   │   └── invite-participants
        │   │   │   │   ├── invite-participants.css
        │   │   │   │   ├── invite-participants.html
        │   │   │   │   └── invite-participants.ts
        │   │   ├── dashboard
        │   │   │   ├── admin-dashboard
        │   │   │   │   ├── admin-dashboard.css
        │   │   │   │   ├── admin-dashboard.html
        │   │   │   │   └── admin-dashboard.ts
        │   │   │   ├── calendar-view
        │   │   │   │   ├── calendar-view.css
        │   │   │   │   ├── calendar-view.html
        │   │   │   │   ├── calendar-view.ts
        │   │   │   │   └── event-details-dialog
        │   │   │   │   │   ├── event-details-dialog.css
        │   │   │   │   │   ├── event-details-dialog.html
        │   │   │   │   │   └── event-details-dialog.ts
        │   │   │   ├── dashboard-layout
        │   │   │   │   ├── dashboard-layout.css
        │   │   │   │   ├── dashboard-layout.html
        │   │   │   │   └── dashboard-layout.ts
        │   │   │   ├── notifications-widget
        │   │   │   │   ├── notifications-widget.css
        │   │   │   │   ├── notifications-widget.html
        │   │   │   │   └── notifications-widget.ts
        │   │   │   ├── overview-page
        │   │   │   │   ├── overview-page.css
        │   │   │   │   ├── overview-page.html
        │   │   │   │   └── overview-page.ts
        │   │   │   └── unified-dashboard
        │   │   │   │   ├── unified-dashboard.css
        │   │   │   │   ├── unified-dashboard.html
        │   │   │   │   └── unified-dashboard.ts
        │   │   ├── matches
        │   │   │   ├── match-details
        │   │   │   │   ├── match-details.css
        │   │   │   │   ├── match-details.html
        │   │   │   │   └── match-details.ts
        │   │   │   └── match-list
        │   │   │   │   ├── match-list.css
        │   │   │   │   ├── match-list.html
        │   │   │   │   └── match-list.ts
        │   │   ├── notifications
        │   │   │   ├── notification-list
        │   │   │   │   ├── notification-list.css
        │   │   │   │   ├── notification-list.html
        │   │   │   │   └── notification-list.ts
        │   │   │   └── request-handler
        │   │   │   │   ├── request-handler.css
        │   │   │   │   ├── request-handler.html
        │   │   │   │   └── request-handler.ts
        │   │   ├── places
        │   │   │   ├── filter-bar
        │   │   │   │   ├── filter-bar.css
        │   │   │   │   ├── filter-bar.html
        │   │   │   │   └── filter-bar.ts
        │   │   │   ├── place-details
        │   │   │   │   ├── place-details.css
        │   │   │   │   ├── place-details.html
        │   │   │   │   └── place-details.ts
        │   │   │   └── place-list
        │   │   │   │   ├── place-list.css
        │   │   │   │   ├── place-list.html
        │   │   │   │   └── place-list.ts
        │   │   ├── teams
        │   │   │   ├── create-team
        │   │   │   │   ├── create-team.css
        │   │   │   │   ├── create-team.html
        │   │   │   │   └── create-team.ts
        │   │   │   ├── invite-player
        │   │   │   │   ├── invite-player.css
        │   │   │   │   ├── invite-player.html
        │   │   │   │   └── invite-player.ts
        │   │   │   ├── team-details
        │   │   │   │   ├── team-details.css
        │   │   │   │   ├── team-details.html
        │   │   │   │   └── team-details.ts
        │   │   │   ├── team-list
        │   │   │   │   ├── team-list.css
        │   │   │   │   ├── team-list.html
        │   │   │   │   └── team-list.ts
        │   │   │   └── team-requests
        │   │   │   │   ├── team-requests.css
        │   │   │   │   ├── team-requests.html
        │   │   │   │   └── team-requests.ts
        │   │   └── users
        │   │   │   ├── profile
        │   │   │       ├── profile.css
        │   │   │       ├── profile.html
        │   │   │       └── profile.ts
        │   │   │   ├── user-card
        │   │   │       ├── user-card.css
        │   │   │       ├── user-card.html
        │   │   │       └── user-card.ts
        │   │   │   └── user-list
        │   │   │       ├── user-list.css
        │   │   │       ├── user-list.html
        │   │   │       └── user-list.ts
        │   ├── home
        │   │   ├── about-section
        │   │   │   ├── about-section.css
        │   │   │   ├── about-section.html
        │   │   │   └── about-section.ts
        │   │   ├── contact-section
        │   │   │   ├── contact-section.css
        │   │   │   ├── contact-section.html
        │   │   │   └── contact-section.ts
        │   │   ├── features-section
        │   │   │   ├── features-section.css
        │   │   │   ├── features-section.html
        │   │   │   └── features-section.ts
        │   │   ├── hero-section
        │   │   │   ├── hero-section.css
        │   │   │   ├── hero-section.html
        │   │   │   └── hero-section.ts
        │   │   ├── home-footer
        │   │   │   ├── home-footer.css
        │   │   │   ├── home-footer.html
        │   │   │   └── home-footer.ts
        │   │   ├── home-navbar
        │   │   │   ├── home-navbar.css
        │   │   │   ├── home-navbar.html
        │   │   │   └── home-navbar.ts
        │   │   └── home-page
        │   │   │   ├── home-page.css
        │   │   │   ├── home-page.html
        │   │   │   └── home-page.ts
        │   └── shared
        │   │   ├── confirmation-dialog
        │   │       └── confirmation-dialog.ts
        │   │   ├── error-demo
        │   │       └── error-demo.component.ts
        │   │   ├── error-notifications
        │   │       └── error-notifications.component.ts
        │   │   ├── not-found
        │   │       ├── not-found.css
        │   │       ├── not-found.html
        │   │       └── not-found.ts
        │   │   └── sidebar
        │   │       ├── sidebar.css
        │   │       ├── sidebar.html
        │   │       └── sidebar.ts
        ├── custom-theme.scss
        ├── index.html
        ├── main.ts
        └── styles.css
    ├── tsconfig.app.json
    ├── tsconfig.json
    └── tsconfig.spec.json
