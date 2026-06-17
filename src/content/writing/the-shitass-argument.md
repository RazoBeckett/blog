---
title: 'The Shitass Argument'
description: "A raw take on tech egos"
heroImage: '../../assets/writing/the-shitass-argument/cover.jpg'
pubDate: 2026-03-21
---

## <i>"I have never seen any system that have DB on another and main application on another"</i>

I have spent a lot of my time building, crafting and more importantly exploring things that actually exist in the tech world. This incident genuinely drove me mad. And honestly you are going to like this because sometimes you just have to say fuck the system.

I am not going to be very specific with names because some people have a heavy ego problem. They will not even try to validate whatever the fuck they say. I hate this mindset because it does not help them grow and it does not let others do their work. Just reading for five minutes could solve the whole argument but instead they choose to waste one hour conflicting with the person who is actually right. This is notoriously bad behaviour.

Just because you THINK whatever you know is the only fact and whatever you know is sufficient does not mean the rest of the world stopped building new systems. People are chatting, reading, experimenting and shipping real things. Those things exist whether you give a fuck about them or not.

---

## The Assignment

So I had an assignment to perform. The idea was to demonstrate a real world failure scenario. The tool to be used was Ansible. Simple enough.

What I did was straightforward. I had two nodes. On one node I deployed the main application. On another node I deployed the database. And do not tell me deployment is not a task. It absolutely is. Infrastructure deployment is literally one of the most real tasks in modern engineering.

Now think logically. What happens if the DB fails. The application cannot fetch data. The service cannot serve users. That is a system failure. That is exactly the kind of situation automation tooling is supposed to handle.

But apparently that was not what they wanted.

They started asking what if it fails later. Show logs. Show recovery. So I did exactly that. I simulated DB failure. I wrote a playbook that extracts logs for inspection. I restored the previous configuration values on the DB node so the system could recover and function again.

**Real scenario. Real debugging. Real recovery.**

And then they say this is not what I meant.

---

## The Moving Goalpost

Now comes a completely unrelated example. Suppose you are a team of three. One person writes document X. Another writes document Y. You as team lead must submit both together. If X does not reach you the process changes.

Wow. Suddenly requirements are changing mid discussion.

So what I did earlier was correct engineering work but still I was told to change it. And when I explained that deploying the application on one node is one responsibility and maintaining the database on another node is another responsibility they hit me again with the same legendary statement.

### "I have never seen any system where DB is separate."

So what now. NeonDB is fake. Managed database services are fake. Microservices architecture is fake. Separation between data layer and application layer is fake.

---

## And let us talk about security for a second.

Why would a hacker even bother tampering with your database if everything is running on the same machine right. Why would anyone design isolation boundaries. Why would anyone reduce blast radius. Why would anyone care about intrusion containment.

Clearly we should just deploy everything on one single node like absolute geniuses.

Application. Database. Logs. Backups. Maybe even production secrets in plain text. Perfect.

We must all be wrong. And these people who have never shipped real production systems must be right.

---

## This is what actually burns my brain.

**Being wrong is fine.**  
**Refusing to learn is not.**

You can spend five minutes reading documentation.  
You can explore one real architecture diagram.  
You can ask one honest question.

Instead some people prefer to defend ignorance like it is their life mission.

This mindset wastes time.  
It slows teams.  
It kills innovation.

Technology moves insanely fast. If you stop exploring you start becoming obsolete.

---

I am not sorry if this hurts someone. If you feel attacked there is a very high chance you belong to this group of people. And if that is the case then stop wasting everyone's time and start learning something useful.
