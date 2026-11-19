# Dar Zitoune | Restaurant Support Assistant

**Author** Khalid Aslaoui (SOOVENSO) · **Brand** SV

An offline prototype for a fictional Casablanca restaurant. Visitors can ask about
the menu, prices and opening times in French or Moroccan Darija. A language
selector controls replies. Unknown requests, allergy questions and reservations
go into an on-page staff queue.

## Run the demo

Open `index.html` in a browser. No install, browser extension or account is required.

| Try | Expected result |
| --- | --- |
| Quel est le menu ? | Three dishes and prices |
| فاش كتحلو؟ | Opening hours in Darija after choosing Darija |
| Ch7al le couscous ? | 55 DH |
| Le tajine de poulet contient-il des noix ? | Staff handoff |
| Livrez-vous à domicile ? | Staff handoff |

## Implementation and scope

The assistant maps supported phrases to a small restaurant catalog with JavaScript.
The menu and business hours are shared with the sidebar. The staff queue is
simulated in the page and resets on reload. The prototype uses no LLM and makes
no network requests. It recognizes a limited set of phrases, and routes requests
outside its reference data to the queue.

A possible next milestone is a real Make webhook that sends staff a handoff
notification and records the review status with permission to use that data.
