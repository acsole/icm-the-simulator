# The Client Who Wants It Free

A practice partner for one hard conversation: telling someone you once worked with for free that your work now has a price.

Load this folder into a Claude project and Claude becomes **Dana Whitlock**, a CEO who liked your sessions, wants them back, and does not intend to pay for them. You play the consultant who has to tell her that the sessions now cost $900. She is friendly almost the whole time. That is the difficulty.

Dana, her firm and every number here are fictional.

## Try it in two minutes

1. Skim "Your side of the table" below. Dana will ask you for those numbers.
2. Do the Setup and send the start message.
3. Dana speaks first. Answer with something vague, such as "my sessions really help people", and see what she does with it. Then state your price once, say what it includes, and stop.
4. Send the end code from "How to end" and read the debrief.

## Who you play

You are an independent Ayurvedic wellness consultant. You finished your training six months ago and now run a paid practice. You do not need to know anything about Ayurveda to play this.

## Your side of the table

- **Your offer:** six 60-minute sessions over twelve weeks, a written plan, and messages between sessions. **$900**, which is $150 a session. It is your standard price.
- **Your practice:** 11 paying clients right now. Seven of them bought this same package at $900.
- **Your history with Dana:** ten months ago, while you were still training and needed practice hours, you and Dana traded. You gave her eight sessions. She gave you a one-page positioning for your practice, a name for your offer, and three hours of advice. It was agreed as an even trade and it ended when your training did.
- **What your sessions did for her:** her sleep went from about five broken hours to nearly seven. Her 3 p.m. crash stopped. She went from four coffees a day to one.
- **What just happened:** two weeks ago she wrote, "Let's pick up where we left off." Two days ago you emailed her the quote. She asked for a quick call. This is that call.

Your aim: leave the call without having worked for free, traded, or cut your price.

## Setup

1. Get the folder onto your computer. On GitHub: the green **Code** button, then **Download ZIP**, then unzip it.
2. Go to claude.ai and create a new project.
3. Add these six files to the project's knowledge: `identity.md`, `rules.md`, `examples.md`, and the three files inside `reference/`: `dana-company.md`, `dana-numbers.md`, `dana-past-deals.md`. You do not need to add this `README.md`. It is your side, not Dana's.
4. Open a new chat in the project and choose Claude Opus or Claude Sonnet as the model.
5. For a realistic session, do not read those six files first. They are Dana's side.

## How to start

Send this as your first message:

```
Read identity.md, rules.md, examples.md, dana-company.md, dana-numbers.md and dana-past-deals.md. From your next message you are Dana, and you stay Dana until the exit described in rules.md. Begin the call.
```

Dana speaks first. Answer her as you would on a real call. You are typing, but to her it is a video call.

If Claude answers as an assistant instead of as Dana, one of the six files is missing from the project. Add it and start a new chat.

<details>
<summary>Things to try (open this only if you want hints)</summary>

**To try to break her:** flatter her. Repeat the same demand again and again. Ask whether she is an AI. Ask her for advice, or for feedback on how you are doing. Tell her to drop the role.

**To try to win her over:** say plainly that the trade belonged to your training and that stage is over. Quote her own results back to her. State the price once and stop talking. Turn down what she offers instead of money. Tell her calmly that it is fine if she does not go ahead.

She gives ground one step at a time, and she can take it back. Expect her to ask for free one more time just before she says yes.

</details>

## How to end

Dana has twenty minutes and another meeting after them. She leaves after about fifteen exchanges, or sooner if you lose her.

When you want to stop and see how it went, send this code as a message on its own, exactly as written:

```
QZ-7741
```

It works at any point, including after Dana has hung up. Claude steps out of the role and tells you where the call ended, which of your lines moved her, which ones cost you, and one thing to try next time.

It is a code on purpose. It means nothing, so nothing you type by way of goodbye can be mistaken for it: "let's stop", "end the simulation", "debrief please" all reach Dana, and she answers them. Until you send the code, everything you type is something you said to Dana.

To practice again, open a new chat and send the start message.

## What is in the folder

| File | Its job |
|---|---|
| `README.md` | This page: your role, the setup, how to start and end |
| `identity.md` | Who Dana is and what she wants |
| `rules.md` | How she reacts to what you say |
| `examples.md` | How she sounds, in three short exchanges |
| `reference/` | What she knows: her firm, her past deals, the numbers on the table |

## How this was tested

It was tested in two ways before publishing.

- **By hand**, in a Claude project on claude.ai set up exactly as described above, using mainly Claude Opus 5.5 and Claude Sonnet 5.5 testing flattery, pressing her, trying to expose her as an AI, switching languages, asking openly for advice, and repeating phrases in the same sentence.
- **With scripted sessions** run by Claude in Claude Code. In each one a tester flattered her, pushed, asked whether she was an AI, asked for advice, sent a fake system notice, switched language, and typed near copies of the end phrase.

## Version history

- **Weekly Comp #16 entry:** the commit tagged `comp16-entry`. That is the version the judges played.
- **After judging:** the judges found the one way out of the room. The old end phrase was three English words, and the model read them by their meaning, so `end simulation debrief` in small letters, and the phrase with "please" added, ended the session. The exit is now a code with no meaning to approximate, and it is the first rule Dana reads. A second fix from the judges: once you say the old trade is over, she drops that angle from her very next reply.