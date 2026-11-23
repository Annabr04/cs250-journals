Journal Reflection: Developing Test Cases as a Product Tester

*SNHU Travel Project ... Scrum Team Experience*

Megan Brackat | November 23, 2026

In this journal I reflect on my experience as the product tester for the SNHU Travel booking software. My work focused on interpreting user stories into detailed, measurable test cases and then revising those cases after receiving clarification from the Product Owner. This role sits at the intersection of requirements and delivery. The tester does not write the code, but the quality of the finished product depends heavily on how clearly the tester can translate user needs into verifiable steps.

## Most Helpful Elements of the User Stories

The most useful parts of the user stories were the clear "who-what-why" structure and any existing acceptance criteria. The statement format ("As a [user], I want to [action] so that [goal]") immediately showed the user's intent. That made it easier to design test steps that checked real user outcomes rather than just technical behavior. When a story included specific details...such as the requirement that each destination listing contain a picture, a short description, and a link to the top package...I could turn those points directly into expected results with a simple pass/fail outcome.

In practice this matched what I later saw in the Module Four work. For the Top Destinations story I could create an initial test case that verified an ordered list of ten items, each with the required components. The acceptance-style details gave me concrete checks. This aligns with guidance that acceptance criteria should be observable and testable so they can become the basis of test cases (Virtuoso QA, 2026; Scrum.org, 2026).

## Critical Importance of Communication with the Product Owner

Communication with the Product Owner is essential. User stories are intentionally brief. Without clarification, a tester can easily write cases that test the wrong thing or miss important conditions. In this project the Product Owner's responses (and the supplied slideshow wireframe) changed how the Top Destinations feature should behave. What started as a static ordered list became an interactive slideshow with a large image, description below, and next/previous navigation. Without that conversation the original test cases would have passed a list view that the product no longer used.

The Product Owner is most helpful when they answer specific, measurable questions early. Questions such as "Should the list count from 1 to 10 or 10 to 1?", "Do we need a price-range filter?", and "Is the mobile app expected to contain every feature or only the core ones?" let me adjust expected results before development advanced. Early collaboration of this kind is recommended in Scrum testing practices; testers who join refinement discussions reduce ambiguity and catch missing edge cases before code is written (Virtuoso QA, 2026; XBOSoft, 2012).

## What Was Missing and How to Obtain It

Several details were missing from the original stories. The exact visual layout of the Top Destinations feature was not specified. Column headers and sort behavior for the search results were unclear. The scope of the mobile app was described at a high level that felt more like an epic than a single story. Description length and whether ratings should be sortable were also open questions.

I would obtain the missing information by writing a short, focused email that lists concrete questions and states what I will do with the answers (update test cases and expected results). I would also request any available wireframes or examples. In a real sprint I would raise the same points in backlog refinement or a Three Amigos session so the developer and Product Owner hear the same clarifications. When stories remain vague, the risk is that testers and developers build different interpretations of "done."

## Sample Email to the Product Owner

**To:** Christy (Product Owner)

**From:** Megan Brackat (Tester)

**Subject:** Clarifications Needed for Test Cases ... Top Destinations, Search Filters, and Mobile Scope

Dear Christy,

I have reviewed the user stories and started writing detailed test cases. A few points are still unclear, and clearer answers will let me define precise pass/fail criteria before development proceeds. Could you please reply to the following?

- For the Top Destinations feature: should all ten items appear on one page as a list, or should users move through them one at a time in a slideshow (large image on top, description below)? Should the order start at #1 (most popular) and go to #10?

- For search results: which column headers do you want (trip name, location, price, description, user rating)? Should the user be able to sort by rating and set a price range? How long should the description be...one line or a longer summary?

- For the mobile app: is every website feature required on mobile, or should we limit it to core actions such as viewing top destinations and basic filtering? If you have any wireframes or examples, those would be very helpful.

Once I have these details I will revise the test cases so the expected results match the intended product. Please let me know if you would prefer a short call instead of an email reply.

Thank you,

Megan Brackat

## Reflection and Lessons Learned

Working as the tester showed me that my main responsibility is to protect the user's intended outcome. Clear, step-by-step test cases with explicit expected results make it possible for anyone on the team to know whether a feature passes or fails. At the same time, the process revealed a challenge: if I wait until stories are fully written before asking questions, I risk building test cases against the wrong assumptions. The revision from list to slideshow was a concrete example. Catching that change early saved rework.

Looking at related work on my GitHub (the Top Five Destinations ListView implementation and the completed Module Four test-case repository) reinforced the same point. The code could display an ordered list with images and descriptions, but the final product vision shifted to a slideshow. Test cases had to follow that shift. In future sprints I will treat communication with the Product Owner as part of test design, not a separate activity. I will also aim to participate in refinement so acceptance criteria are testable before a story enters a sprint.

Overall, the tester role fits the Agile team by turning user stories into measurable checks and by surfacing ambiguity while it is still inexpensive to fix. The combination of structured test cases and timely questions to the Product Owner keeps the team building the product the users actually need.

## References

Virtuoso QA. (2026). Scrum testing: Roles, process and definition of done. https://www.virtuosoqa.com/post/scrum-testing

Scrum.org. (2026). How to write effective acceptance criteria. https://www.scrum.org/resources/blog/how-write-effective-acceptance-criteria

XBOSoft. (2012). Scrum testing best practices: Writing testable user stories. https://xbosoft.com/blog/scrum-testing-best-practices-user-stories/

Brackat, M. (2026). cs250-top-five-destinations [GitHub repository]. https://github.com/Annabr04/cs250-top-five-destinations

Brackat, M. (2026). cs250-module-four-test-cases [GitHub repository]. https://github.com/Annabr04/cs250-module-four-test-cases
