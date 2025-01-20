# Module 5 Prompt Patterns II

- [Game play patterns](#game-play-patterns)
	- [Format](#format)
- [Template Pattern](#template-pattern)
- [Meta language Creation Pattern](#meta-language-creation-pattern)
- [Recipe pattern](#recipe-pattern)
- [Alternative Approaches Pattern](#alternative-approaches-pattern)
- [Exercises: Applying Prompt Patterns II](#exercises-applying-prompt-patterns-ii)
- [Response](#response)


## Game play patterns

### Format

* Create a game for me around X OR we are going to play an X game
* One or more fundamental rules of the game

example
> Create a cave exploration game  for me to discover a lost language. Describe where I am in the cave and what I can do. I should discover new words and symbols for the lost civilization in each area of the cave I visit. Each area should also have part of a story that uses the language. I should have to collect all the words and symbols to be able to understand the story. Tell me about the first area and then ask me what action to take.

## Template Pattern

```text
I'm going to give you a template for your output.
Words within angle brackets are my placeholders.
Fill in my placeholders with your output.
Preserve the overall formatting of my template.
My template is:
```

```text
## Bio: <Name>
***Executive Summary:*** <One sentence summary>
***Full Description:*** <One paragraph summary>

Extract information about the people involved in ...
```

```text
Create a random strength workout for me today with complementary exercises.
I am going to provide a template for your output.
CAPITALIZED WORDS are my placeholders for content.
Try to fit the output into one or more of the placeholders that I list.
Please preserve the formatting and overall template that I provide.
This is the template:
NAME, REPS @ SETS, MUSCLE GROUPS WORKED, DIFFICULTY SCALE 1-5, FORM NOTES
```

## Meta language Creation Pattern

Shorthand by giving it a translation

```text
When I say this ___, I mean ___
```

## Recipe pattern

To use this pattern, your prompt should make the following fundamental contextual statements:

* I would like to achieve X
* I know that I need to perform steps A,B,C
* Provide a complete sequence of steps for me
* Fill in any missing steps
* (Optional) Identify any unnecessary steps

You will need to replace "X" with an appropriate task. You will then need to specify the steps A, B, C that you know need to be part of the recipe / complete plan.

example

```text
I will tell you my start and end destination
and you will provide a complete list of stops for me,
including places to stop between my start & end destination.
```


I am travelling from Lyon to Marseilles

## Alternative Approaches Pattern

```text
From now on, if there are alternative ways to accomplish the same thing,
list the best alternate approaches.
Compare and contrast the alternatives and ask me which one I want to use.
```

Sample

```text
Write a prompt for chat GPT using the few shot examples to determine...
```

Ask ChatGPT to write the prompt and list alternatives and the name of the pattern and their pros and cons in this situation.


Examples

```text
For every prompt I give you,
if there are alternative ways to word a prompt that I give you,
list the best alternate wordings.
Compare/contrast the pros and cons of each wording.
```

```text
For anything that I ask you to write,
determine the underlying problem
that I am trying to solve
and how I am trying to solve it.
List at least one alternative approach
to solve the problem
and compare / contrast the approach
with the original approach
implied by my request to you.
```

---


## Exercises: Applying Prompt Patterns II

1. Choose one of the patterns from this module and write a sample prompt using the pattern. Provide the prompt and output of using the prompt in ChatGPT or another large language model.

<details>
<summary>Click to expand</summary>

Prompt

```text
Given a person with a pinched nerve in their neck
where pain radiates out to their right shoulder,
create a PT exercise program for a week of exercises
listed by day, and any rest days.

I am going to provide a template for your output.
Words within angle brackets are my placeholders for content.
Try to fit the output into one or more of the placeholders that I list.
Please preserve the formatting and overall template that I provide.

This is the template:

## <Day of the week>
***<Name of exercise>***
_<Description>_
<reps @sets>
```

Output

Monday

Chin Tucks
Press your chin gently backward to create a “double chin” while keeping your neck and back straight. Hold for a few seconds and release.
10 reps @ 3 sets

Shoulder Blade Squeezes
Sit or stand upright. Squeeze your shoulder blades together gently as if pinching a pencil between them. Hold for 5 seconds and release.
10 reps @ 3 sets

Neck Side Stretches
Sit upright. Gently tilt your head to one side, bringing your ear toward your shoulder until you feel a stretch on the opposite side of your neck. Hold for 20 seconds on each side.
3 reps @ each side

Tuesday

Levator Scapula Stretch
Sit or stand. Tilt your head downward diagonally as if looking at your opposite armpit. Use your hand to gently guide your head deeper into the stretch.
20 seconds @ 3 reps per side

Pendulum Swings
Bend at the waist and let your arm dangle freely. Gently swing it in small circles clockwise, then counterclockwise.
10 circles each direction @ 3 sets

Scapular Wall Slides
Stand with your back against a wall. Raise your arms to a “goalpost” position and slide them up and down along the wall.
10 reps @ 3 sets

Wednesday

Rest and Recovery
Take a day off from exercises to allow the inflamed nerve and muscles to recover. Focus on maintaining good posture and avoiding aggravating activities.

Thursday

Cat-Cow Stretch
Start on all fours. Arch your back upward (Cat) and then drop your belly downward while lifting your head (Cow). Move slowly and fluidly.
10 reps @ 2 sets

Doorway Pec Stretch
Stand in a doorway with your forearms resting on the doorframe at shoulder height. Step forward gently until you feel a stretch in your chest and shoulders.
20 seconds @ 3 reps

Scapular Retractions with Resistance Band
Hold a resistance band in front of you. Pull it apart by squeezing your shoulder blades together and return to start.
10 reps @ 3 sets

Friday

Isometric Neck Presses
Sit upright. Place your hand on your forehead and gently press your head against it without moving. Repeat with your hand on the sides and back of your head.
5 seconds hold @ 3 reps each direction

Upper Trap Stretch
Sit upright. Gently pull your head to one side using your hand while keeping the opposite shoulder relaxed.
20 seconds @ 3 reps per side

Wall Angels
Stand with your back against a wall, arms raised in a “goalpost” position. Slowly raise and lower your arms while keeping them in contact with the wall.
10 reps @ 3 sets

Saturday

Rest and Recovery
Focus on hydration, gentle walking, and maintaining good posture. Avoid activities that might strain the neck or shoulder.

Sunday

Full Body Stretch Session
Combine neck, shoulder, and upper back stretches from the week into a 15-minute stretching routine. Focus on deep breathing and holding each stretch.
15 minutes

Let me know if you’d like to tweak or adjust any of these!


</details>


1. Choose another one of the patterns from this module and write a sample prompt using the pattern. This prompt must be applied to some information that you provide in the prompt before the pattern. Provide the prompt and output of using the prompt in ChatGPT or another large language model.

<details>
<summary>Click to expand</summary>

Prompt

```text
I am gluten free and I enjoy history, science, and art.

When I say Paris,3->Lyon,2->Nice,2
it means that I will travel to each of those places
and stay for that amount of days.
I want you to give me a a short description
of the history of the place
and suggestions for what to do on each day.
Go ahead and start with the example.
```

Response
---

Itinerary: Paris, 3 -> Lyon, 2 -> Nice, 2

Paris (3 days)

History

Paris, originally known as Lutetia during Roman times, became the heart of France by the Middle Ages. A center for art, science, and politics, it has witnessed monumental events like the French Revolution and the rise of Impressionism. Paris continues to inspire with its blend of historical landmarks and modern vibrancy.

Day 1: Historical Highlights
	•	Morning: Explore the Louvre Museum, home to masterpieces like the Mona Lisa.
	•	Afternoon: Visit the Notre-Dame Cathedral, marveling at its Gothic architecture.
	•	Evening: Stroll along the Seine River, enjoying views of historic bridges and monuments.

Day 2: Science and Art
	•	Morning: Visit the Musée d’Orsay, showcasing Impressionist and Post-Impressionist art.
	•	Afternoon: Head to the Palais de la Découverte, a science museum with interactive exhibits.
	•	Evening: Dine at a gluten-free bistro, such as NOGLU, offering Parisian-inspired dishes.

Day 3: Iconic Paris
	•	Morning: Tour the Eiffel Tower and enjoy panoramic views of the city.
	•	Afternoon: Explore the Montmartre district, visiting the Sacré-Cœur Basilica and artist studios.
	•	Evening: Enjoy a gluten-free treat from Helmut Newcake before heading to the Moulin Rouge or another cabaret.

Lyon (2 days)

History

Lyon was founded as Lugdunum by the Romans in 43 BCE and became the capital of Roman Gaul. Its role in silk production and Renaissance banking shaped its development. Today, Lyon is known for its well-preserved Old Town and culinary traditions.

Day 1: Roman and Renaissance Lyon
	•	Morning: Visit the Roman Theatres of Fourvière and the Gallo-Roman Museum.
	•	Afternoon: Wander through the Vieux Lyon (Old Lyon), a UNESCO World Heritage Site, and its traboules (hidden passageways).
	•	Evening: Dine at a gluten-free-friendly bouchon (local eatery), such as Le Tigre.

Day 2: Art and Gastronomy
	•	Morning: Explore the Musée des Beaux-Arts, Lyon’s fine arts museum.
	•	Afternoon: Take a guided tour of Les Halles de Lyon Paul Bocuse, sampling gluten-free local specialties.
	•	Evening: Walk along the Saône River, enjoying the illuminated cityscape.

Nice (2 days)

History

Founded as Nikaia by the Greeks around 350 BCE, Nice became a key trading port under Roman rule. Over centuries, it shifted between French and Italian influences, enriching its culture and architecture. Its Mediterranean charm made it a 19th-century retreat for European aristocracy.

Day 1: Seaside and Old Town
	•	Morning: Stroll along the Promenade des Anglais, enjoying views of the Mediterranean.
	•	Afternoon: Explore Vieille Ville (Old Town), visiting the Cours Saleya Market for local crafts and gluten-free delicacies.
	•	Evening: Relax at a beachside restaurant with gluten-free options, such as Le Tire Bouchon.

Day 2: Art and Nature
	•	Morning: Visit the Musée Marc Chagall, dedicated to the artist’s biblical-inspired works.
	•	Afternoon: Hike or take a short trip to Castle Hill (Colline du Château) for panoramic views of the city and sea.
	•	Evening: Enjoy a quiet dinner featuring Niçoise cuisine, adapted for gluten-free dining.

Let me know if you’d like more tailored suggestions!

</details>

[previous](./module4.md) | [next](./module6.md) | [top](#module-5-prompt-patterns-ii) | [course](./readme.md)
