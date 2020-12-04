# Pivit's Brain dump

### Why is this an issue?
There is nothing better than getting a new project cloned, running the tests, knowing everything is working correctly, then you can do your dev, and check against those tests.
We all know TDD is good, but with the Magento Core team, it seems that the emphasis is on end-to-end testing, that's why there are so many integration tests and very few unit tests when it comes down to it.

When pulling down a project and you run the unit tests and a bunch fail, it then becomes VERY difficult, if not impossible to get the same confidence in the modifications you are writing.

The point of this repository is to maintain and coordinate the volunteer efforts of all of us looking to make Magento Open Source a stable platform, and hopefully catch a few problems before they become problems.

### How do we tackle such a beast
My thoughts on this are there are really two issues to address here:
1. Existing tests are failing
2. Writing Unit tests is tedious in the Magento framework

#### Existing tests are failing
Ideally we can solve this issue by putting some dev effort into modifying the unit tests so that they pass. If old code is being used, we can use our mind powers to figure out why and fix it. Once we get these tests to a stable point, the unit tests can be used before merging in pull requests the same way the integration and static tests are being conducted currently

#### Writing Unit tests is tedious in the Magento framework
Well this one is a difficult one to aproach, but I for one am a huge fan of automating mundane repetitive tasks. It would be awesome to have IDE plugins or something that point out the test coverage, generate test classes based on existing classes (or vice versa if people actually did TDD)
These are things that aren't necesary but could definitely aid in making writing unit tests a joy rather than a chore at the end because we were told we needed to have testing.

Here's just a few of my thoughts to try and get the ball rolling.
