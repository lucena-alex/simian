# Simian! :banana::monkey_face::point_right:    :point_left::monkey_face::moneybag:

This project is an attempt at modelling the fundamental, abstracted forces of an economy by simulating the base principles of exchange. 

I'm at least temporarily naming it "simian" because "simulated economy" lead me to "sim. econ." and that lead me to think of how neat it is that we, among all our primate cousins, were sophisticated enough to arrive at this mess : )

## Goals

With this project, I'd like to:

1. Make a little gadget to play with to experiment with economic ideas. Outside of industry tools (market analytics, supply chain management tools, proper fintech stuff), there doesn't seem to be a ton of interactive tools to doing so. What I have been able to find are more like illustrations of "applied sciences", basically business training. Interestingly I've found mention of a few interesting simulations (including a few by the ECB!) from the Adobe Flash era that are basically lost to history (as far as I care to search : ) )

2. One possible proper _use_ for this gadget that I'd thought of was as a tool to balance game economies in their design stage. A tool to give you some empirical-ish numbers for how many gil that rare armor should cost in relation to the health potion to feel believable / satisfying. Committing to this as a goal definitely implies some big design decisions I'm not ready to make yet, but I would like to project to remain as modular as necessary to keep that door open in the future.

## Motivations

I am far from the most well-studied amateur economist, but I do like reading up on the topic. I like how powerful minds throughout human history have grasped to make sense of the relationships between work, wealth, nature, and human society, and even though these questions are as old as we are, and basically span a big chunk of the human condition altogether, it feels incredibly hard to make sense of from within the thing.

I've always liked parametric / procedural / generative programs that take some rules and made-up values as input and output something unexpected. I feel that a tool into which you can communicate an intention and get a result that feels familiar but not completely controlled by your intention, is a very evocative thing! Almost an artistic process. Neat!

Combining the two, I thought it would be neat to have an incredibly abstracted economic model to play with ideas in both domains. I've found it surprising, if not a little disappointing, that in this age of generative AIs, neural networks, GPU-hyper-optimized simulations and whatnot, the field of economics hasn't made a ton of use of these tools to study economies in the abstract. Maybe understandably, economists more often like to set computers to crunching numbers to forecast future conditions, rather than as little Petri dishes. I think this is a shame, particularly given that practically every field of academic study has forged exciting new tools out of these digital materials in my lifetime alone!

## Tech

This is currently writing with .NET, just because it's what I use most for work, and I happen to think it's very nice. My current plan is to develop the core simulation first, then sit a little server with an API on top, then give it a simple web UI for development. I might use GraphQL for the interface, just because I like it and would like to work more with it. I will probably use Blazor for the UI, just because it'll be simplest for me for development.

## "Roadmap"

Here are a number of spitball-ed ideas for future features/elaborations/levels of complexity I'd like to incorporate into this model one day.

- Some way of representing inter-national relationships / exchange
- Add more types of agent-entities. Entities that do banking, entities that do credit/lending.
- Add a mechanism for governmental action. Things like laws and "policies", i.e. "the monetary unit is changing", "taxes will now exist", "central bank will now touch the big INTEREST RATE lever in their office". These would be driven by simulated agents independent of the user, rather than just being input parameters.
- I think the first pass at the UI will be super tabular, dry and boring, but eventually it would be fun to generate newspaper covers of the little simians' goings on : ) This might necessitate like an introspection / analytics engine as part of the sim, that could look at the state of the model and draw interesting insights to remark upon, like "gold has been supplanted by bananas as the national currency"