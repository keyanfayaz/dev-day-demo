# DevDay demo

An interactive conversation replay for a DevDay meetup talk about Homie, my Dot, helping prepare Raidio's production setup on a Mac mini.

## Presenting

Open `index.html` in a browser. Everything, including Homie's avatar, is embedded in that file. No installation or internet connection is required.

- Click the thread or the **Continue…** prompt to reveal the next moment.
- **Space**, **Enter**, or **Right arrow** advance. **Left arrow** goes back.
- **F** enters full screen.
- Work tabs appear separately with a spinning indicator, then complete on a later click.
- Chapter 1 ends with a separate click that adds a thumbs-up reaction to the sushi pickup message. Continue clicking to start chapter 2.
- Chapter 2 ends with a separate click that sends “Let’s do it” in response to Homie's MacBook Pro suggestion.
- Use the **Replay** button in the top right to start again.

The typing indicator waits 2.5 seconds after the first message from Me. All conversation messages wait for a click.

## About the story

Raidio is an AI radio app I developed on my MacBook Pro. I wanted to run its production setup on my Mac mini while testing the idea. Homie helped review the plan, told me when to switch the connected computer, and continued checking the mini's actual setup.

The replay uses selected excerpts from that conversation. The beta checks passed, while a production or TestFlight release was still pending in the messages shown.

The chapters use **Oct 3** and **Oct 4** date labels. Chapter 2's date and request to test and benchmark the mini for the Base model appear together on one click. The benchmark message quotes the supplied Oct 13 screenshot: 5.66 seconds to generate 4 seconds of audio after warmup, about 71% of the required speed, roughly 42% more throughput needed, and 97.5% of the time spent on model computation. With the current implementation, the mini could not sustain continuous Base generation.

The date labels follow the requested presentation timeline. The chapter 2 connecting request, acknowledgment, and suggestion to benchmark the MacBook Pro are reconstructed for the presentation. The MacBook Pro proposal still needs a performance test.

The conversation, styling, and interactions are all editable in `index.html`.
