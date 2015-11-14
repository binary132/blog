+++
Categories = ["Mindfork", "Go"]
Description = "The rebirth of Mindfork"
Tags = ["Mindfork", "Go", "Dash", "Gatekeeper", "SynapseGarden"]
date = "2015-02-10T20:47:50-05:00"
menu = "Mindfork"
title = "Rebirth of Mindfork"

+++

Today is the day I renew my work on [Mindfork](https://github.com/mindfork).

<!--more-->

# Why?

Mindfork began as an idea for a calendar or todo app which keeps track of performance or other metrics, offering the user guidance toward goals.  It quickly evolved into much more, but was never completed beyond a few quick sketches.

Mindfork is meant not just to help people work together, but to help us learn together.  In university, I never learned about the "Real World" ecosystem of tools and ideas until I pursued that knowledge for myself, and there's no roadmap.  At all.  A huge goal of Mindfork is to bring people with different knowledge together to create a community where what needs to be learned can be learned.

Today, the idea of a resume-as-a-service reminded me of the user skills tracker I imagined as a core feature of Mindfork.

## Toxic Culture

Coming out of school, I quickly realized that the Real World of software engineers isn't a curious place full of learning; it is *brutally cutthroat*.  The culture in some communities is completely toxic, save for a very few people.  Many engineers and sysadmins seem to exist solely for the purpose of aggrandizing themselves at the expense of others, belittling and mocking the less talented or knowledgeable, and creating cults around arcane and extreme code cultures.

The *culture du jour* is a moving target; one can never strive to become excellent in it without being seen as a hapless follower, hopelessly behind the times as the Gnostic wizards of code pursue ever more obscure, powerful solutions to problems that may or may not ever exist.  And of course backlash cultures then spring into existence, equally bigoted and ignorant with an equally pompous attitude towards the hopelessly un-hip.

## Ignorance

There seem to be thousands of such systems and tools, and communities revolving around them.  In today's industry, finding a job often seems to be less about being a good engineer, and more about being good at guessing what trends are trendiest.  Most of us in the software world don't even need me to give a few examples; Big Data is a catchword which seems to constantly roll out of the mouths of the ignorant, along with other phrases, such as "webscale", "enterprise", and so on.  (Am I, too, guilty of mockery and elitism?  Perhaps a bit.)

# The Solution

I began working at DigitalOcean in June of 2013.  I was incredibly excited.  This was it.  I was getting involved in the hot stuff.  I felt like I'd won the lottery.  I was full of fire and love for the product, and for life; my daughter had been born just a week or two before, I'd just moved across the country, and I was full of the dream that I could achieve whatever I set my heart and mind to.  So I did.  I threw myself head-on into learning everything I could about distributed systems and new ideas about concurrent programming, with tools like Go, Erlang (which was experiencing a minor resurge in popularity), and Scala.

I had access to free cloud hosting, and I was liberal with trial credits.  I was highly involved with the community.  I've always been a person who loves teaching and learning, and I was available to communicate with people who came to me with questions.  And I was learning, too.

## Community Power

I saw the vast potential of the community organized around learning together.  I saw that with huge numbers of people, we could accomplish nearly anything imaginable.  It was just a question of how; humans aren't fast enough or smart enough to manage projects at that scale unless it's their full-time job, and such jobs don't come easily with free software.

Now, with cheap clusters at our fingertips in the cloud, we had tools powerful enough to manage thousands of people, working together in real time.  We had tools we could all work on, together, using DCVS like Git.  And we had tools which could really perform, in concurrency-oriented runtimes like Go and Nodejs, and datastores we could put enormous amounts of data in.

We just needed the software to do it.  That idea was born as Mindfork.

It was a very *webscale* moment in the *big data cloud*.

# Origins and Progress

Today, I started on the first working agent, a simple login service called [Gatekeeper](https://github.com/mindfork/gatekeeper).  Together with [Kevin Weber](http://bluevisual.tv), I'm building a web dashboard framework, [Dash](https://github.com/synapse-garden/dash), in tandem with Mindfork, so that they can grow and evolve together, giving users easy access to the early power of Mindfork.  Dash is the software which powers [synapsegarden.net](http://synapsegarden.net).

The purpose of Mindfork is to create a framework for automated community collaboration, centered around free software.  Mindfork is *free* software (see [here](https://www.gnu.org/philosophy/free-sw.html) for a meaningful definition of *free*) which intelligently manages data.  Anyone can run it and use it.  It is at heart all about free exchange of ideas, to create a new ecosystem where people collaborate to gain power, instead of competing.

SynapseGarden is the learning, growing, collaborative community which will be built around Mindfork.

# Mindfork Basics

A Mindfork cluster is built out of simple "Agents" which each have a single responsibility, and communicate with each other over the network to find out what they need to know.  Agents can be forked (copied) and built upon, and new improved Agents given back to the ecosystem; clusters of Agents can create a holistic view of data, giving the owner and users insight and projections.

The purpose is to create an analytic suite for communities of humans.  How do people work best?  Maybe some people work best in the morning, and some work best at night.  Maybe some people work best with others, while others work best alone.  Mindfork helps us ask and answer these kinds of questions.

For now, the only question it will answer is, "are you logged in?"

More to come.
