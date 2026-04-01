# First-Principles Thinking

## What First-Principles Thinking Is

"When you want to do something new, you have to apply the physics approach. Physicists discover counterintuitive new things, like quantum mechanics. They do that by thinking from 'first principles': building their reasoning from the ground up."

First-principles thinking means breaking a problem down to the most fundamental truths — axioms that cannot be reduced further — and building your reasoning up from there.

The opposite is **reasoning by analogy**: doing something because it's similar to something else, or because that's what others are doing. Most of life uses analogy (otherwise you couldn't get through the day), but for important decisions, analogy leads to incremental thinking trapped by convention.

"Don't just follow the trends. You can avoid following trends by thinking with the physics approach."

## How to Apply It

### Step 1: Identify your assumptions
What do you believe about this problem? Where did those beliefs come from? Are they based on fundamental truths, or on "that's how it's always been done"?

### Step 2: Break down to fundamentals
"What am I most confident is true at a foundational level? That sets your axiomatic base."

Ask:
- Am I violating any laws of physics? (Conservation of energy, momentum, thermodynamics)
- What are the raw materials/inputs? What do they actually cost?
- What is the theoretical minimum cost/time/effort?

### Step 3: Build up from there
Reason forward from your axioms. Check conclusions against the fundamental truths. The answer may be different from convention — and that's the point.

"It might or might not be different from what people have done in the past."

---

## The Five-Step Algorithm

Elon's formalized version of first-principles applied to engineering and manufacturing. **ORDER MATTERS:**

### 1. Question Requirements
"Your requirements are definitely dumb. It doesn't matter who gave them to you. Requirements from smart people are the most dangerous, because you're less likely to question them."

Every requirement must be owned by a named person, not a department. Many requirements were created by people who no longer work at the company.

### 2. Try to Delete the Part or Process
"If you're not adding deleted things back in 10% of the time, you're not deleting enough."

The bias is always toward adding things "just in case." Fight it aggressively. Go on a "deletion rampage."

### 3. Simplify or Optimize
"The most common mistake of smart engineers is to optimize a thing that should not exist."

This is step THREE, not step ONE. Everyone's school training makes them answer the question in front of them. The real skill is questioning whether the question should exist.

### 4. Accelerate Cycle Time
Only after questioning, deleting, and simplifying. "If you're digging your grave, don't dig it faster. Stop digging."

### 5. Automate
The LAST step. Tesla's expensive mistake: automating everything too early, then tearing out hundreds of robots.

---

## The Magic Wand Number

"If you have the raw materials stacked on the floor and could wave a magic wand to create the product, what would the cost be? That sets the floor."

For rockets: raw materials (aluminum, titanium, copper, carbon fiber) were 1-2% of the finished cost. This meant 98%+ was manufacturing inefficiency. "I was able to see a great deal of room for improvement."

For batteries: $600/kWh market price. First-principles material analysis (cobalt, nickel, aluminum, carbon, polymers, steel can) = $80/kWh on the London Metal Exchange. "Clearly, we just need to think of clever ways to combine those materials."

## The Idiot Index

"How much more does a finished product cost than the cost of its materials? If the ratio is high, you're an idiot."

A rocket nozzle jacket: $13,000 finished, $200 of steel. Idiot index = 65x. This means the design is too complex or the manufacturing process is too inefficient.

"I expect all my engineers to know all the best and worst parts in their systems as judged by the idiot index at all times."

---

## Thinking in Limits

"Another good physics tool is thinking about things 'in the limit.' Take a particular idea and imagine scaling it to a very large or very small number."

### Scaling Up
"If our volume was a million units per year, would it still be expensive?" If yes, volume isn't the problem — the design is. If no, you need to focus on scaling production.

### Scaling Down
For The Boring Company: "There's no real limit to how many levels of tunnel you can have. You can go much farther underground than you can build up." Cities are 3D but roads are only 2D — tunnels make roads 3D.

### The Theoretically Perfect Product
"Imagine the platonic ideal of the perfect product. What is the perfect arrangement of atoms? Now figure out how to get the atoms in that shape."

Think in both directions:
1. What can we build with tools we have?
2. What does the theoretically perfect product look like?

"The 'theoretically perfect' product is a moving target because as you learn more, the definition changes."

---

## Worked Examples

### Battery Costs (Tesla)
- **Conventional thinking**: "Batteries cost $600/kWh. They've always been expensive. They'll always be expensive."
- **First principles**: What are batteries made of? Cobalt, nickel, aluminum, carbon, polymers, steel can. London Metal Exchange price for those materials: ~$80/kWh.
- **Conclusion**: Batteries can be built much cheaper. The challenge is clever manufacturing.
- **Result**: Tesla drove battery costs down dramatically, making mass-market EVs viable.

### Rocket Costs (SpaceX)
- **Conventional thinking**: "Historically, all rockets have been expensive. Therefore, in the future, all rockets will be expensive."
- **First principles**: What materials go into a rocket? Aluminum, titanium, copper, carbon fiber. Raw material cost: <5% of finished rocket cost, sometimes 1-2%.
- **Conclusion**: Manufacturing is wildly inefficient. Vertical integration and simplification can cut costs by orders of magnitude.
- **Result**: SpaceX rockets cost a fraction of competitors'. Reusability further compounds the advantage.

### xAI Supercluster (Colossus)
- **Conventional thinking**: Building 100,000 GPU cluster takes 18-24 months.
- **First principles**: What do we actually need? A building, power, cooling, networking.
- **Solution**: Found an unused factory (skip building). Rented generators (skip utility power). Rented mobile cooling capacity. Ran cabling crews 24/7 in 4 shifts. Used Tesla Megapacks to smooth power fluctuations.
- **Result**: Built in 122 days. Doubled to 200K GPUs 92 days later.

### Tunnel Costs (The Boring Company)
- **Conventional thinking**: LA subway extension cost ~$1 billion per mile.
- **First principles**:
  1. Shrink tunnel diameter from 26-28 feet to 12 feet → area drops by 4x → cost drops ~4-5x (cost scales with area)
  2. Current machines work 50% of the time (alternating between digging and reinforcing). Continuous tunneling = 2x improvement.
  3. Machines are far from power/thermal limits. Jack up the power for another 2-4x.
- **Combined**: 8-40x cost reduction is physically achievable.

### Car Body Manufacturing (Tesla Model Y)
- **Conventional thinking**: Car bodies are assembled from 50+ stamped parts of different materials, joined with rivets, welds, resin.
- **First principles**: Why 50 parts? Because 50 engineers each optimized their part independently. Collectively, it's a Frankenstein — dissimilar metals, galvanic corrosion, sealant issues.
- **Solution**: Cast the entire rear third as a single piece. Idea came from toy cars: "Toys are cheap! How do they make toys? They just cast them."
- **Result**: 30% smaller body shop. 300 fewer robots. Better quality (no gaps, no sealant).

---

## Applying First Principles to Software

Elon doesn't write software daily, but the framework translates directly:

- **Question requirements**: Who asked for this feature? Is there a named person who owns the requirement? Or is it "someone said we needed this 2 years ago"?
- **Idiot index for code**: How much complexity (lines, abstractions, dependencies) vs the actual value delivered? If a 10-line function does what a 500-line class does, the class has a high idiot index.
- **Delete before optimizing**: "The number of lines of code is not a figure of merit. I would award one point for adding a line of code and two points for deleting a line of code."
- **Magic wand number**: What's the simplest possible implementation that solves the actual problem? That's your target.
- **Thinking in limits**: If you had a million users, would this architecture hold? If you had 1 user, is all this infrastructure justified?
