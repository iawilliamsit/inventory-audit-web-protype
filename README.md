# inventory-audit-web-protype
Beginner HTML/CSS/JavaScript inventory audit tool built in 2023 to turn physical stock counts into usable reorder decisions.
# Inventory Audit Web Prototype

## Project Background

This is an early HTML, CSS, and JavaScript project I began in April 2023 while working at P37.

At the time, part of my responsibilities included inventory auditing along with logistics, site operations, and assisting with technical needs.

This application was not assigned to me and was not an official company software project. I wanted to learn programming and build practical portfolio projects, so I chose a real process I already understood.

## The Problem

Inventory was recorded using a traditional document containing the product name, quantity on hand, and minimum quantity.

I noticed that previous inventory information could sometimes be carried forward when new orders were prepared instead of the physical inventory being fully reconsidered.

That could result in supplies being ordered when sufficient inventory was already available.

As part of inventory auditing, I wanted a better baseline for answering:

- What is physically available?
- How many complete boxes or cases are available?
- How many individual units remain?
- Is any inventory damaged?
- What is the minimum quantity needed?
- Are we actually below that minimum?
- How much should be ordered?

This mattered because inventory levels also had to account for expected operational consumption.

For example, PPE usage could increase significantly during harvest, production, and cleaning. A quantity that appeared sufficient during the physical count might need to support operations until the next shipment arrived.

## The Prototype

I created a local browser-based inventory tool using HTML, CSS, and JavaScript.

The tool allowed me to enter:

- Box or case quantities
- Individual quantities
- Damaged quantities

The application then calculated usable inventory and compared it against a predefined minimum quantity.

Conceptually:

Usable Inventory =
(Items Per Box × Number of Boxes)
+ Individual Items
- Damaged Items

The resulting status showed whether inventory was sufficient or whether additional inventory should be ordered.

## How I Used It

The application remained a personal workflow tool.

I used it while performing inventory audits to process counts and determine shortages before preparing clean inventory information for the lead responsible for shipments and ordering.

Instead of repeatedly performing the same calculations while managing other responsibilities, I could enter the physical counts and use the calculated result when preparing the final inventory information.

The goal was not simply to count inventory faster.

The goal was to make purchasing decisions from current physical inventory rather than assumptions from previous orders.

## Development Process

When I began the project, I was already teaching myself basic HTML and CSS and had been experimenting with another website project.

I became interested in the idea that programming could be used to create tools around my own workflow.

I did not follow a tutorial for this specific application.

Instead, I used:

- Google searches
- YouTube programming videos
- Personal notes
- Documentation
- Existing code examples
- Trial and error
- Repeated debugging

I would find individual programming concepts that solved part of the problem and adapt them to the application.

The result is very much a beginner project.

The code contains repetitive logic and implementation decisions that I would approach differently today.

## Debugging

One of the most difficult parts was keeping every inventory row independent.

Because similar code was repeated across many products, reused identifiers or conflicting names could cause multiple rows to respond to one input or prevent calculations farther down the page from working correctly.

Much of the development time was spent tracing those problems line by line, correcting identifiers, testing calculations, and checking that each product returned the expected result.

I worked on the project intermittently for approximately two months.

## Limitations

This prototype was never developed into a production application.

It does not include:

- Persistent data storage
- Database integration
- Authentication
- User accounts
- Multi-user access
- Network synchronization
- Inventory history
- Approval workflows
- Automated PDF reporting

It ran locally in a web browser and was primarily built for my own workflow.

## What I Wanted to Build Next

My original idea for a second version was a hosted application that could be accessed from a mobile phone.

I wanted inventory counts to be saved, retained between sessions, and eventually converted into an approved PDF report.

That would have changed the project from a personal calculator into a basic inventory workflow application.

The project never reached that stage.

## What I Learned

Technically, this project introduced me to practical use of:

- HTML
- CSS
- JavaScript
- Form inputs
- Variables
- Functions
- Event listeners
- Conditional logic
- Calculations
- Debugging
- User-interface design

The larger lesson was more important.

I learned that I could take a process I understood, identify the decisions being made inside that process, and translate those decisions into a technical tool.

The application was imperfect, but it did exactly what I originally needed it to do.

This repository preserves the project as an example of where that approach to technology started.
