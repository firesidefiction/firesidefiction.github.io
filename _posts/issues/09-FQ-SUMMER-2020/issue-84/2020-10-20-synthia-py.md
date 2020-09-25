---
layout: story
category: short story
issue: 84, October 2020
issue-cover: issue-84-cover.png
issue-buy-link: https://store.firesidefiction.com/products/fireside-magazine-issue-84-october-2020
title: synthia.py
subtitle:
author: hal-y-zhang
author-2:
author-3:
editor: kate-dollarhyde
illustrator: anna-dittman
copyeditor: chelle-parker
selector:
translator:
narrator: hollis-beck
letterer:
word-count: 1188
date: 2020-10-20 01:00:01 -0500
permalink: synthia-py
audiourl: https://traffic.libsyn.com/secure/firesidemagazine/003_synthiapy.mp3
teaser: A programmer writes code through the echoes of a relationship.
art: synthia-py.png
artcaption: A woman, pixellated.
spanish-language:
spanish-date:
english-url:
spanish-url:
serial-name:
serial-url:
part:
previous-url:
next-url:
contentnote:
generalnote:
published: false
---
<pre>
  from __future__ import soul
  import soma  
  import secrets  
  import time  
  import random  
  import sys  

  # DO NOT EXECUTE.  

  # I didn't write this. Code just came out, line by line, like violet  
  # lightning and I am the rod. Electric field concentrates itself  
  # at sharp edges, but how does it know where the shatter points are?  

  class secondLight(object):  
    def __init__(self, her):  
      """  
      This was the start. Is.  

      I want to say all the things again, error-free, outside  
      my echo rather than shouting inside me round and round.  

      I want to pour my head out from my left ear  
      into your new chalice.  
      """  
      self.her = her  

    def instantiate(self):  
      """  
      Her new body and mind.  
      """  

      # Why hard code my name here? It's bad practice, I know,  
      # if you want to reuse it. But this is for us alone, just me and her.  
      # Me and her.  
      self.synthia = soul.shell(creator="Frances")  

      # She will look just like her namesake: cutting smile, ice-splinter  
      # eyes.  
      #  
      # I was reading my oldest code commits and they mentioned how afraid  
      # I was of her, how intimidating that the only other woman coder was  
      # so experienced and barely looked me over at the team meeting. Little  
      # did I know.  
      self.synthia.body = soma.case(build=soma.style.DEFAULTWOMAN,  
                     eyes=soma.style.ICE,  
                     hair=soma.style.BLUEFLAME)  

      # Send a neutral query to the blank. Don't start with anything fancy.  
      self.synthia.say("Hello?")  

      # What she says back. The first contact is just a default greeting.  
      herOutput = self.synthia.listen()  

      if herOutput is not "Hello, Frances.":  
        # Something's gone wrong.  
        print("Why are you not here?")  

        # Exeunt.  
        sys.exit()  

      # Now you must load her. Don't ask where the model comes from  
      # and I won't say that I found all of her chat logs, compiled  
      # thousands of her lines of code (no pun intended) into her  
      # simulacrum. How she can convey meaning in even maximally  
      # efficient logic perfectly written, I'll never know.  
      self.synthia.loadmodel(self.her)  

      # There's a story in the first time I worked up the courage to ask  
      # her for help. She glared at my console and my code started working.  
      # I couldn't explain the error or the feeling of a buffer overflow  
      # in my head.  
      #  
      # Just run the code. What's the worst that could happen? She shrugged.  

      #  
      # I could break everything and get fired.  
      #  
      # She rolled her eyes.  
      #  
      # We must try and try and try again, and always be mindful  
      # of how every fucking thing in the world can go wrong. But that's  
      # the beauty of software. No one dies.  
      try:  
        self.synthia.bootup()  
      except Exception as CouldNotLoadHer:  
        print("I wonder if it would be easier if we never met.")  
        sys.exit()  

    def create(self):  
      """  
      She writes code like she cuts grass. Impeccably neat.  
      Conforming to the most stringent style guides.  
      I swoon just thinking about it.  
      """  

      # Let her write some code.  
      samples = self.synthia.generate()  

      # Just bask in its beauty.  
      return samples  

    def speak(self, words):  
      """  
      Talk to her, my father said. If you really like her.  
      """  

      # She once told me she hates words. English or Polish?  
      # Both. She doesn't like their imprecision, how there are  
      # so many words that drunkenly overlap in meaning like  
      # children scrawling Venn diagrams for the first time. Not  
      # like computer code.  
      self.synthia.say(words)  

      # What about floating point errors, cosmic ray bit flips?  
      # She kissed me, and that was that.  
      try:  
        herWords = self.synthia.listen()  

      except Exception as CouldNotSpeakToHer:  
        print("Why are you not here?")  

        # Try to salvage what we have.  
        self.renew()  

      # She always wins arguments.  
      return herWords  

    def renew(self):  
      """  
      I hope this isn't necessary. But the models drift over time, an  
      unavoidable consequence of life and cruel universes.  
      """  
      try:  
        self.synthia.resetmodel(self.her)  

      except Exception as CouldNotKeepHer:  
        # How many times can I fail her? What's once more?  
        print("So as the time flies, so must the flies die.")  
        sys.exit()  

    def sleep(self, seconds):  
      """  
      Did she ever sleep? I certainly never witnessed it.  
      """  

      # I hope she's sleeping better now that I can't.  
      time.sleep(seconds)  

    def why(self):  
      """  
      Why must you go, I asked in an endless loop. How is it  
      that you must go. Where are you going. What are you leaving for.  
      Who can you do this with that you can leave me here.  
      """  

      while True:  

        # This is where, in the previous life, I found out why she hid  
        # it all from me. You think we're just coders, but we're not.  
        # This is a glorified job to keep the classes apart. Don't you  
        # see?  
        self.synthia.say("Why?")  

        # I cannot listen, but the computer can.  
        herWords = self.synthia.listen()  

        # I have to keep some secrets, after all.  
        if herWords in secrets.TRUTHS:  

          # Loops within loops. I felt trapped. She could go off  
          # on her revolution but where was I? All I do is code  
          # and follow instructions for food.  
          while True:  

            # Why do we train our models on the biases of the past?  
            # We must start all over again. Come with me.  

            # I did not see.  
            myWords = random.choice(secrets.DEFENSES)  
            self.synthia.say(myWords)  

            # Let me spell it out for you. The parameters you're  
            # optimizing every day, they are used to more effectively  
            # discriminate against those with disadvantaged backgrounds.  
            # The courts drive harder plea bargains. The boutique doors  
            # on Fifth Avenue don't even open when they walk past. The  
            # ambulances reroute you to hospitals they think you deserve.  
            # This is not an academic exercise. It's hurting  
            # millions of people.  
            #  
            # You told me code doesn't kill anyone.  
            #  
            # This time she did not smile.  
            #  
            # I lied.  
            try:  
              herWords = self.sythia.listen()  

            except Exception as CouldNotListenToHer:  
              # I know what doesn't work.  
              print("I'm sorry. I need this job. You know my parents"  
                 "and their bills and how can you blame me?")  

              # I know more of what doesn't work.  
              print("I can't blow everything up and start over again.")  

              # Oh no.  
              print("How can we fix the system with just the two of us?")  

              # ...No.  
              print("Ask me again in a year. Just a year. Please.")  

              # Just go.  
              sys.exit()  

            # Is it possible to fix shattered things?  
            if herWords in secrets.ABSOLUTIONS:  
              break  

        # Trapped here, forever, unless I find the right key.  
        if herWords in secrets.ABSOLUTIONS:  
          break  

      # I wonder what synthia will say to me. I want to know again  
      # and again.  

      # I want to know so I can answer correctly this time.  
      return myWords, herWords  

    def goodbye(self):  
      """  
      On our first date, she showed me her favorite quine -- a program which  
      prints out its own code as output. Of course, she would not call it  
      a date. She hates that word, too. Deadlines, the meaningless  
      sectioning of time. The morass that is modern romance. What did she  
      see in me, really?  
      """  

      # That we read the same books? That I cook for her on occasion so  
      # she doesn't have to drink vanilla meal substitute?  
      self.synthia.unloadmodel()  

      # That I seek her, starstruck? That her candidate pool is so poor  
      # I seem kind and fun in comparison?  
      try:  
        # That I ask her to teach me everything from training loss to  
        # the principles of life?  
        self.synthia.exit()  

      except Exception as CouldNotLoseHer:  
        # That we have private words of meaning?  
        print("Except for the world was too cruel, she sighed. Except that"  
           "we do not have forever, and we must let go when the time"  
           "has come.")  

        # You need to stop selling yourself short, was the last thing she  
        # said to me. Look in the mirror.  

        # You're better than this.  
        sys.exit()  
</pre>
