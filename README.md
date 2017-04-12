# TimeTravellingTelephone

Dr. Bill Turkel’s Interactive Exhibit Design is a graduate level course at Western University in London, Ontario, Canada. The course is briefly summarized as:

"History 9832B is a studio course on interactive exhibit design, intended primarily for public historians and digital humanists. Students will learn how to create interactive exhibits through a series of hands-on projects that teach the basics of interaction design, physical computing, and desktop fabrication."

Unlike anything the authors of this paper have ever experienced in academia, this short report chronicles our time in Bill Turkel’s lab as well as the creation of our final project: The Time Travelling Telephone.

The Journey from Paper Toys to Programming.

The idea for a time travelling telephone, with which you dial a date and transport yourself to another era through the timeless medium of music, evolved partly out of the course objectives and partly out of a series of under-developed, over-confident, and ultimately unsuccessful ideas. It was through these first fruitless attempts that we discovered our creative and technical limits. But we also discovered how to push these limits.

Day 1: Kyle says to Bill “I really want to learn to code. HTML, CSS, C+, Python, Processing - I don’t know where to start but I know I want to learn to code.” In response, Bill says “Here, borrow my ‘Introduction to Processing’ book and in 10 years you’ll be an expert programmer.” Little did we know it at the time, but the genesis for our project began here in this short exchange.

As the course got underway, each week we were introduced to new tools and technologies with regards to interactive exhibit design.

Our first idea came when working with MakeDo and storyboarding our idea to demonstrate to the others. The idea was simple, a toaster that could toast a portrait of any pre-programmed historical figure you like. We called it “The Historical Toaster.” Though this idea persisted throughout the duration of the course, we did not have the means or expertise to make our cardboard prototype a reality.

We then moved into working with electronics and digital devices. We were running Processing and Arduino while using Phidgets sensors. Generally just playing with our environment through the variety of sensors provided by Phidgets. While most people would not consider this to be overly sophisticated technology, it was brand new territory to us. It helped us consider what kind of interactions we could include in our final project (light sensors, pressure sensors, motion sensors, buttons, etc.). Ultimately, Processing and Arduino became major parts of our final project.

While working with electronics we were introduced to Little Bits. Little Bits uses a battery to power various controls (dials, buttons, etc.) and outputs (light, sound, motors). We made up the CircleDrawer3000, a machine that had a motor, a wheel, and a marker and could draw while moving in circles. While this was not a groundbreaking invention, the creative process introduced us to messing around with electronics - something we would have to do with our rotary phone.

After working with electronics and digital devices the course returned to more low-tech instruments of interactive exhibit design. We experimented with paper folding and mechanical design. While working with paper, cardboard, VEX, and MicroRax kits, we were essentially just playing around; in the most scientific sense of the phrase, of course. We made a boat, a box, a moveable cartoon clip, a metal frame, and a rube goldberg machine.

The Time Travelling Telephone: Our Final Project

Quite frankly, when it came time to finally decide on a final project we were at a loss for ideas. A few of the projects we considered were ‘Guerilla History’ and a ‘Counterfactuals Game.’ The objective of Guerilla History was to create a sticker which could be placed at historically significant sites and triggered by motion or the press of a button. This would activate an audio clip revealing an aspect of history lesser known to the public. These stickers could be reprogrammable and placed anywhere by the user. But it proved far too ambitious and less interactive than we hoped. The Counterfactuals Game would present an alternative outcome of history depending on the move players made. For example, if the user chose to make the D-Day landings on coast of Northern Germany, would the results have been different? Well, you would have to play the game to find out. This too, though, proved to be an overly complicated idea. We revisited the Historical Toaster as well but quickly saw it was far too complex a project for us to undertake.

At this point, we realized we had to return to basics and focus on interactions that we could build our project around. That’s when we started wondering, what could we do with a rotary phone? We were both drawn to the nostalgia that a rotary phone offered. Interacting with a phone is intuitive - the process of dialing is something that everyone is familiar with, So we asked ourselves, what is natural for a phone? The answer, we thought, was to listen. ‘Listen to what?’ was our next question. That was when we decided to use the rotary phone as a mechanism to listen to music.
	
We first sought to replicate the experience of a rotary phone with a circular-touch Phidget. The problem here was that our computers failed to recognize the device and all attempts to resolve this failed. It also did not evoke the experience and vintage flair that people would get from using a rotary phone. We then turned our attention to the online market places of eBay, Craigslist, and Kijiji. Eventually, we found a vintage rotary phone on Kijiji for twenty-dollars, sold locally by a man who went only by the name Dan. He advertised himself as “The best store online.” This was the phone for us. 

We quickly bought the phone and took it back to Bill Turkel’s lab to take it apart and begin our build. At this point, we had just two classes left to complete the project.

The Build

Step 1: Deconstruct the phone to isolate the rotary dialer.

Step 2: Connect the rotary dialer to the Arduino processor and connect the processor to the computer.

Step 3: Develop a code to download onto the Arduino that would allow it to transform the analog signal of the phone into a digital signal that could be read by the computer, so that dialing “4” on the phone would make a “4” show up on the computer.

Step 4: Develop a code which would allow Arduino to talk to Processing, triggering an audio file to play at Arduino’s request. This process was at its core a series of “If” statements. If “4” is dialed, then play audio file number 4.

Step 5: Choose which music to play with the phone and create short audio clips using Audacity sound editing software.

Taking the phone apart and connecting it to Arduino were the most straightforward parts of the project. Luckily this is a process that others have undertaken and shared online, and we were able to use these guides. Developing code to do exactly what we wanted was considerably harder. Here, too, we were lucky in the sense that others had shared their attempts online. However, nobody had programmed their phones to do precisely what we wanted ours to do. Given our minimal experience programming, the biggest obstacle to realizing our plans was developing a code that would play music based on the phone’s input. We spent a lot of time researching, combining, writing, and testing codes, but none of them were successful. Ultimately, what we came up with is a ‘Franken-code’ of sorts: borrowing bits of code from online sources and Processing textbooks, and tweaking it ever so slightly to perform as we needed. We then simply housed the entire build in the original rotary phone frame (removing the original insides).

For the music the phone would play, we decided to use the top-selling singles of the 1970s. It is a decade with some seriously catchy tunes, and is also a time when people actually used rotary phones. We found the top single for each year of the 70s (ten songs total), and edited them down to a shorter length so users would not have to stand there listening for 3-4 minutes at a time. We also found clips of Casey Kasem introducing these songs on his radio show “America’s Top 40” and blended them with clips of the music to create short, fifty-second audio clips. His introductions provide some historical context for the songs and artists. The phone works as such: A visitor walks up to the phone, chooses a number from the directory, dials the number, and listens to the corresponding song; introduced by legendary radio host Casey Kasem

All code is available, free to use, and attached to this page in the form of .txt files.
