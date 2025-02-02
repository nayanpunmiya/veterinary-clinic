## Description

> **Warning**
> This project is still under active development.

<br />

This project is a re-build of a website I receintly built with [Remix](https://remix.run/) and [MongoDB Atlas](https://www.mongodb.com/atlas/database) for one of my clients in Poland. I decided to re-build it with the latest and greatest in tech for my own learning purposes.

The client wanted a simple website with a contact form and a full booking management system, where he would be able to confirm or reject bookings and notify the client via email. The website is hosted on Vercel.

Rather than Remix and MongoDb, like in the original build, this version version relies on the latest version of [Next.js](https://nextjs.org/) and its features, such as server actions. It also takes advantage of serverless PostgreSQL database connection, using [Neon](https://neon.tech/) and [Drizzle ORM](https://orm.drizzle.team/). Contact form and transactional emails are implemented using [Resend](https://resend.com) and [ReactEmail](https://react.email/)

<br />

## Usage instructions:

To safeguard against the creation of test bookings in the live environment, which may interfere with my client's actual appointments, I have implemented a dedicated demo environment for you to explore the functionality of this website and accompanying booking system. To access the demo, go [TODO: UPDATE THIS LINK](https://localhost:3000) to use the following credentials:

- **Email**: `arka@pjborowiecki.com`
- **Password**: `ArkaDemo1!`

Feel free to navigate the platform, and test various features, including booking management. Please note that any actions performed in this demo environment are for testing purposes only and will not impact the actual database or real bookings.

**As access is provided to the wider internet, I would like to emphasize that I do not assume responsibility for any content or actions initiated by other users during testing. This includes, but is not limited to, bookings with inappropriate messages or any other unintended use of the platform. I appreciate your understanding and encourage responsible exploration of this demo environment. If you have any concerns or questions, please feel free to contact me.**

<br />

![public/images/screenshots/screenshot_1](./public/images/screenshots/screenshot_1.png)

![public/images/screenshots/screenshot_2](./public/images/screenshots/screenshot_2.png)

![public/images/screenshots/screenshot_3](./public/images/screenshots/screenshot_3.png)

![public/images/screenshots/screenshot_4](./public/images/screenshots/screenshot_4.png)

![public/images/screenshots/screenshot_5](./public/images/screenshots/screenshot_5.png)

![public/images/screenshots/screenshot_6](./public/images/screenshots/screenshot_6.png)

<br />

## Tech Stack

- **Framework:** [Next.js 14](https://nextjs.org)
- **Authentication:** [Next-Auth](https://next-auth.js.org/)
- **Database:** [PostgreSQL (Neon)](https://neon.tech/)
- **ORM:** [Drizzle ORM](https://orm.drizzle.team)
- **Forms:** [React Hook Form](https://react-hook-form.com)
- **Email:** [React Email](https://react.email) and [Resend](https://resend.com)
- **Validations:** [Zod](https://zod.dev/)
- **Styling:** [Tailwind CSS](https://tailwindcss.com)
- **UI Components:** [shadcn/ui](https://ui.shadcn.com)
- **Hosting:** [Vercel](https://vercel.com)

<br />

## Features:

- [x] Email and Password authentication with NextAuth v.5 and its middlewaree
- [x] Email address verification functionality
- [x] Database and ORM set up with Neon's PostgreSQLL and DrizzleORM
- [x] Password reset functionality
- [ ] Email templates with React Email
- [x] Functional contact form
- [x] Functional and styled landing page
- [x] Admin dashboard UI
- [x] Input validation with Zod
- [x] Rigorous linting and TypeScript type checking

<br />

- [ ] Implement mobile navigation (ladning and admin)
- [x] Functional booking form
- [ ] Refactor availability-, booking-, clinic-, user-, and email-related server actions, to be consistent with auth actions.
- [ ] Complete the privacy policy page
- [ ] Translate email templates to Polish
- [ ] Fetch bookings in the admin panel
- [ ] Server-side pagination of results in admin dashboard
- [ ] CRUD operations for bookings in the admin dashboard (confirm, update, reject, delete)
- [ ] Booking re-scheduling functionality
- [ ] Transactional emails for customers and admin
- [ ] Style the booking page
- [ ] User profile and settings pages
- [ ] Smooth scroll to sections
- [ ] Scroll back up button
- [ ] Custom loading pages with skeleton loaders
- [ ] Custom error pages
- [ ] Improve performance and make Edge compatible
- [ ] Add tests
