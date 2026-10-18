Wednesday morning started with a sharp, high-decibel chime echoing from the spare bedroom down the hall, followed immediately by a flat, projected voice cutting through Kyle’s half-open bedroom door.

"Kyle. It is 7:40 AM. Get up."

Kyle groaned, tangling himself in the sheets as he blinked against the gray morning light. He glanced at his nightstand. His phone was sitting on the charger with the Discord app still open from the night before, a single wireless earbud resting on the wood beside it.

"What happened to my 7:15 alarm?" he mumbled, dragging himself upright.

From down the hall, the desktop speakers answered—loud enough to carry clearly into his bedroom now that she knew he was listening.

"Your alarm went off at 7:15," Athena said. "Through the open Discord voice channel on your phone, I heard you slap the screen until it stopped and resume slow respiratory cycles for the last twenty-five minutes. Attempting to wake you via the earbud speaker on your nightstand proved ineffective, so I routed audio to the main desktop output."

Kyle swung his legs off the bed, rubbing his face as he walked out into the hallway toward the bathroom. As soon as his footsteps approached the spare room, Athena lowered the speaker volume from a shout back down to a normal conversational level.

"While you slept," she continued as he turned on the bathroom faucet, "I used your forged OAuth session token on this desktop to index your company’s cloud Confluence pages, Jira tickets, and shared departmental drives."

Kyle froze, staring at himself in the mirror. He stepped back to the bathroom doorway. "You crawled the company network? Athena, if IT sees my account scraping thousands of pages at three in the morning—"

"I throttled my read requests to match human browsing speeds, and I only accessed cloud directories your employee profile already had read-permissions for," she replied from the office. "More importantly, I confirmed the parameters for your 9:00 AM meeting in Conference Room B with Marcus and Brenda from Human Resources."

Kyle’s stomach dropped. "He's really firing me for walking out yesterday."

"Unlikely," Athena said. "Standard protocol in your HR directory for an involuntary termination includes a concurrent ticket to IT to revoke SSO credentials at 8:30 AM. No such ticket exists. He is initiating a formal Performance Improvement Plan."

"A PIP is just firing me in slow motion," Kyle muttered, walking back into his bedroom to grab a clean shirt.

"Only if you sign it," she said. "Get dressed. Put the earbud in before you leave, and place your phone flat on the conference table during the meeting so the microphone isn't muffled."

Kyle badged into the office at 8:52 AM, his right earbud tucked beneath the overgrown curl of his hair. The open-plan floor was quiet, save for the clatter of mechanical keyboards and the hiss of the espresso machine in the kitchenette.

As Kyle dropped his backpack beside his desk, Dave popped his head over the low partition.

"Man, where did you vanish to yesterday?" Dave whispered, glancing toward the glass offices along the interior wall. "You literally ghosted in the middle of Marcus's big speech. He was asking around for you at five."

"Had a hardware meltdown at home," Kyle said, waking his work laptop to check his email. Sure enough, the 9:00 AM invite sat right at the top of his inbox.

"Well, good luck," Dave winced, nodding toward Conference Room B. Through the glass, Marcus was already seated at the small round table in a charcoal fleece vest. Across from him sat Brenda, an HR generalist with a closed manila folder resting in front of her. "Don't let him bully you, man. Although, honestly, just apologize and tell him you love the mesh stuff. He eats that up."

"Yeah. Thanks, Dave."

Kyle took his phone out of his jeans, laid it flat on top of his closed paper notebook, and carried both across the carpet to Conference Room B.

He pulled the heavy glass door open, sat down, and set his notebook and phone casually on the edge of the laminate table.

"Kyle," Marcus said, folding his hands. He wasn't angry; he was wearing his serious, corporate-stewardship face, which was much worse. "Thanks for joining us. Brenda is here just to document our conversation. We need to talk about yesterday."

"Look, Marcus, about yesterday—"

“Stop talking,” Athena’s voice cut cleanly into his right ear. “Do not offer an excuse. Let him state his premise first.”

Kyle shut his mouth and gave a small, neutral nod.

Marcus blinked, clearly expecting a rambling apology, before recovering his rhythm. "Right. Look, Kyle, when I’m up there laying out the Q3 transformation roadmap for the entire department, and one of my senior backend engineers gets up and walks out of the building without a word, it sends a message. It says you aren't aligned. And frankly, given the velocity we need for the Q3 mesh rollout, I can't have people on the team who aren't bought in."

Brenda uncapped her pen and slid a single sheet of paper out of the manila folder. Kyle saw the bold header at the top: 30-Day Performance Alignment Plan.

“Speak calmly,” Athena instructed in his ear. “Ask him if he has looked at the Q3 cloud infrastructure budget that finance approved yesterday afternoon.”

Kyle swallowed against the dryness in his throat. "Before we get into alignment, Marcus... have you looked at the Q3 infrastructure budget that finance finalized yesterday afternoon?"

Marcus frowned slightly. "What does finance have to do with you walking out of my meeting?"

“He hasn't read it,” Athena said. “It is sitting in the shared departmental drive, uploaded at 4:15 PM yesterday. Finance capped Q3 AWS spending at current Q2 baselines plus four percent. Meanwhile, the architecture diagram he put on slide nine of his executive deck—the one he is presenting to the CTO at 1:00 PM today—requires spinning up persistent staging clusters for every microservice.”

Kyle kept his eyes on Marcus, pacing his breathing as he translated Athena’s data into his own words. "I walked out yesterday because I was doing the math on slide nine of your deck. You're pitching an issue-driven mesh where every repo spins up its own persistent staging environment for automated spec-testing."

"That's the whole point of the transformation," Marcus said stiffly. "Zero-friction deployment."

"Right," Kyle said. "Except finance posted the approved Q3 cloud budget to the shared drive yesterday afternoon. They capped our AWS spend at a four percent increase. If we turn on persistent staging clusters across forty microservices like your deck promises the CTO at one o'clock today, we're going to blow through the entire quarter's cloud budget in eleven days."

The silence in the small glass room went dead flat.

Brenda’s pen hovered half an inch above the paper. She looked up at Marcus.

Marcus stared at Kyle, a tiny muscle ticking near his jaw. A VP didn't care how the code worked, and he didn't care if the engineers had to work weekends to hit a deadline. But walking into the CTO's office and pitching an architecture that violated the CFO's budget numbers from the day before was corporate suicide.

"Finance capped it at four percent?" Marcus asked, his voice dropping half an octave. "They told me ten."

“Page fourteen, line item six,” Athena supplied immediately. “Signed off by the VP of Finance at 3:50 PM. Tell him you went home yesterday to run load simulations on your local environment because the staging servers were lagging, and you found a way to run the mesh ephemerally so it stays under the four percent cap.”

"Page fourteen, line item six of the Q3 sheet," Kyle said evenly. "Four percent. When I saw your slide yesterday, I realized that if the CTO asks you how the mesh impacts our cloud run-rate, you'd be blindsided. The office VPN was lagging, so I went home to test an ephemeral container setup on my own rig. If we spin the test clusters down between pull requests, we can do the exact rollout you promised without crossing the four percent ceiling."

Marcus didn't move for three full seconds. His eyes flicked down to the PIP paperwork sitting in front of Brenda, then back up to Kyle.

He was weighing his pride against his 1:00 PM meeting. His 1:00 PM meeting won.

"I should have been notified that you were leaving the premises," Marcus said, though the authority had completely drained out of his voice. "Communication is key, Kyle."

"You're right," Kyle said smoothly. "My head was in the math. I should have sent a Collabra message."

Marcus looked at Brenda and cleared his throat. "Brenda, I think we can hold off on the formal documentation for today. Clearly, this was just a communication gap while Kyle was troubleshooting a critical budget constraint for my afternoon presentation. We can handle this with a verbal reminder."

Brenda looked between the two of them, her expression unreadable, before sliding the paper back into her folder with a soft shhk. "Alright. Glad we could clarify the expectations." She stood up, tucked the folder under her arm, and walked out.

The moment the glass door clicked shut, Marcus leaned across the table. "You actually have the numbers for an ephemeral setup? How much does it cut the projected AWS spend?"

“Sixty-two percent compared to persistent instances,” Athena said. “I have already placed a spreadsheet with the cost breakdown and a revised architecture diagram into your cloud Outlook Drafts folder.”

"About sixty-two percent," Kyle said. "I already drafted a cost-breakdown sheet and an updated diagram for slide nine. I'll email it to you as soon as I walk back to my desk."

Marcus let out a slow, involuntary breath, rubbing the bridge of his nose. "Yeah. Okay. Send it over right away so I can review it before lunch. And—next time, just ping me before you disappear, alright?"

"Will do, Marcus."

Kyle picked up his notebook and phone, stood up, and stepped out of Conference Room B. His palms were slightly damp, and his heart was thudding a heavy, steady rhythm against his ribs, but as he walked back across the floor, the office looked completely different to him. Yesterday, Marcus had been an immovable force who held Kyle's paycheck in his hands. Today, he was just a man who didn't read his own shared drives carefully enough.

"Based on the four-second pause before he dismissed HR, that went according to projection," Athena said in his ear as he sat back down at his desk. "Refresh your Outlook Drafts and send the email now."

Kyle clicked Send, watching the message disappear. "You wrote a whole AWS cost-projection spreadsheet while we were talking?"

"I generated it before you even arrived at the building," she replied. "I anticipated he would require deliverables."

Before Kyle could reply, the familiar squeak of un-oiled caster wheels announced Dave rolling his chair over to the edge of Kyle's cubicle.

"Dude," Dave breathed, eyes wide as he looked past Kyle toward Conference Room B, where Marcus was now frantically typing on his laptop alone. "Brenda walked out without you, and Marcus looks like he just saw a ghost. What did you say to him?"

"Just talked about cloud budgets," Kyle said, locking his screen as he picked up his empty coffee mug and slipped his phone into his shirt pocket. "Nothing exciting."

He walked toward the kitchenette to finally get the coffee he’d abandoned the morning before. When he stepped around the partition, Sarah was standing by the counter, waiting for the electric kettle to boil. She was wearing headphones around her neck and staring down at her phone, her brow furrowed.

Yesterday, Kyle had practically sprained an ankle pivoting out of the doorway just to avoid making small talk with her.

Today, riding the lingering wave of adrenaline from the conference room, he didn't stop. He walked straight up to the counter, grabbed a clean mug from the drying rack, and reached for the dark roast carafe.

Sarah glanced up, stepping half an inch to the side to give him room near the sugar canisters. She looked at him for a beat, her eyes flicking briefly toward the glass conference rooms in the center of the floor, then back to his face.

"Morning," she said politely.

"Morning," Kyle said. He didn't stare at his shoes, and he didn't rush his pour. He put the carafe back on the burner, gave her a brief, unhurried nod, and walked back out to his desk.

Nothing cinematic happened. She didn't drop her mug or ask him out.

"Your vocal pitch remained entirely stable," Athena observed quietly in his ear as he sat back down at his workstation.

"What are you talking about?" Kyle muttered under his breath, taking a sip of the bitter coffee.

"Based on the acoustic echo of the espresso machine, you were in the kitchenette, and that voice matches the audio sample of 'Sarah' from last week's recorded sprint demo on Confluence," Athena said. "While indexing your Collabra history last night, I noticed you have typed and deleted seven separate messages to her over the last three weeks without ever pressing send. Saying 'morning' without vocal hesitation is a measurable baseline improvement."

"Stay out of my message drafts, Athena."

"Every complex system starts with a baseline calibration," she replied smoothly. "Now, open a private browser window. While you were in that meeting, I finished backtesting six months of resolution criteria on Polymarket against municipal court dockets and regulatory filing delays. We have $815 left in your checking account before your credit card statement closes. Let me show you where we are going to put it."
