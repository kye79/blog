---
title: "My attempt at a versioning system"
author: Kalcor
date: 2018-08-14T16:25:25+03:00
draft: false
---

# Introduction

If you have ever heard of SA-MP (San Andreas Mutliplayer), you might be familiar with the versioning system that I have created.

In my opinion, this versioning system is way better than Semver (Semantic Versioning) and any other versioning system out there.

# So how does it work?

Versioning starts at ***0.0*** and should be at ***0.1*** once it’s usable and ready for the public.

## Major releases

Every time you release a new major update, you increment the second number in the version by one. So for example : ***0.1*** turns into ***0.2***, ***0.2*** turns into ***0.3*** and so on…

The first number in the version is unused and is there purely for looks. Do not change it, as it will not look good.

## Minor releases

Have you written a couple of new functions or fixed one or two bugs here and there and decided to release a minor release? Well that’s just great!

There are two ways to mark minor versions.

The first way is to add a hyphen, followed by the character “R” and the minor release number. (Minor release numbers start from 1)
For example, let’s say the current version is ***0.1***. If you were to release your first minor release it would become ***0.1-R1***. Pretty straight-forward, right!?

The second way is to add a letter at the end of the version if it’s not present already, and increment it if it is. So ***0.1*** with a patch becomes ***0.1a***. ***0.1a*** with another patch becomes ***0.1b***.
However, the English alphabet only contains 26 letters. What do I do once I reach “z”?
Well, that’s pretty simple. Append another new letter to the end. Thus, ***0.1z*** will become ***0.1za*** and so on…

Lets say you had issues learning the alphabet back in primary school, you can simply skip almost the entire alphabet and go from “d” to “x”. This is also perfectly valid.

Now, which one should I choose?
The answer is very simple, choose whatever you want. And feel free to switch between the two whenever you want, this won’t cause any confusion what so ever. If you feel like it, you can even use both at the same time (***0.3zb-R28***). All of this is perfectly valid. Personally, I prefer using both. As that way you can make sure that people who don’t know the alphabet will know what the current minor release is and vice versa.

## Release candidates

Have you written tons of new features and fixed tons of bugs but are worried your obsessed fans that just can’t get enough of you won’t enjoy them? Well then it’s time for a Release candidate!

Release candidates are marked by a hyphen followed by “RC” and the release candidate number.

Release candidates come after minor releases.

## Branching

Let’s say your obsessed fans completely hate your release candidates, but you still want to keep them! You can move all the RC’s into a new branch.

Release candidates are marked by a hyphen followed by a dot followed by whatever you want to call the branch in all caps. The branch name comes after the major release number.

Let’s say the current version is ***0.3zb-R28-RC6***. And you’d like to move all of the release candidates to another branch. ***0.3zb-R28-RC6*** would become ***0.3.-BNzb-R28-RC6***. (With BN being the branch name) It is best to keep branch names at around 2-3 characters, but there is no limit.

Any type of release is allowed to break backwards compatibility. Unlike in Semver, where you are only allowed to break backwards compatibility on major releases. This is one of the many advantages Kalver (Kalcor Versioning) has over Semver.

# A very important DON’T

Do NOT go over 0.3. Getting to major release 4 brings bad luck to your project and certain death to the developers involved. If you want to keep releasing updates at that point, release minor updates.

# In conclusion

In conclusion, kalver is probably the best versioning system you’ll every come by.
I’m right. And if you think that I’m wrong, you’re wrong.