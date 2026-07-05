# The Forgotten Files — Bellingcat Open Source Challenge Write-Up

This write-up covers my process for solving five separate challenges from the Bellingcat Open Source Challenge by Peter Barth, each one testing a different OSINT skill: geolocation, archive digging, and cross-referencing historical records. Some of these took minutes, others took hours of dead ends before the right lead showed up. Below I've broken down each case individually — the clues, the tools I used (Google Maps, Google Dorking, and old newspaper archive sites), and the reasoning that got me to the final answer.

---

## 1. The Saltwater Secret

![ss_photo1](THE_FORGOTTEN_FILES_PHOTOS/the_saltwater_secret/ss_photo1.png)

**Task:** What is the address of this foreign government building (omit 'road, 'avenue', 'street', etc)?

The first thing I did was search:

```
"Billy Barron" AND "1958" AND "Massachusetts"
```

The first result is a pdf file titled "A Disturbing Discovery at Bass Rocks".

The pdf contains the story of Billy Barron and his sister Susie finding a box containing lots of weapons and ammunition.

![ss_photo3](THE_FORGOTTEN_FILES_PHOTOS/the_saltwater_secret/ss_photo3.png)

Just from the title I know that this is on Bass Rocks, Massachusetts, and I immediately searched it on google maps.

![ss_photo4](THE_FORGOTTEN_FILES_PHOTOS/the_saltwater_secret/ss_photo4.png)

My first instinct was to find a small cave-like structure in the area. It took me hours finding a small cave-like structure in the area, but I couldn't find one. I gave up and checked the PDF file again. I noticed that the cover page of the PDF looks familiar.

I noticed that the background looks similar to the area so I tried finding the spot.

![ss_photo5](THE_FORGOTTEN_FILES_PHOTOS/the_saltwater_secret/ss_photo5.png)
![ss_photo6](THE_FORGOTTEN_FILES_PHOTOS/the_saltwater_secret/ss_photo6.png)

**Actual Spot:** https://maps.app.goo.gl/zNqvNuD5kuTT9cct7

The objective is to find a foreign government building, but all I saw was just a bunch of houses. So I searched it on the internet.

![ss_photo7](THE_FORGOTTEN_FILES_PHOTOS/the_saltwater_secret/ss_photo7.png)

The result gave me Sherman Cottage and it turns out it's just near the spot. 24 Bass Rocks Rd.

![ss_photo8](THE_FORGOTTEN_FILES_PHOTOS/the_saltwater_secret/ss_photo8.png)
![ss_photo9](THE_FORGOTTEN_FILES_PHOTOS/the_saltwater_secret/ss_photo9.png)

**Answer:** 24 Bass Rocks

---

## 2. A Hitman's Hobby

![hh_photo1](THE_FORGOTTEN_FILES_PHOTOS/a_hitman's_hobby/hh_photo1.png)

**Task:** What was his hobby?

Just searching Tommy Gibbs gives you lots of results (Tommy Gibbs is a surprisingly common name), so in order to narrow down my search I did a bit of Google Dorking.

![hh_photo2](THE_FORGOTTEN_FILES_PHOTOS/a_hitman's_hobby/hh_photo2.png)

The first thing that comes up, surprisingly, is an article by Peter Barth.

![hh_photo3](THE_FORGOTTEN_FILES_PHOTOS/a_hitman's_hobby/hh_photo3.png)

After reading through the article I found out that Tommy Gibbs' real name is Paul Adams Gibbs. He uses two aliases "George Edward Thomas" & "Tommy Gibbs". Also linked in the text is an old prisoner-run newspaper.

![hh_photo4](THE_FORGOTTEN_FILES_PHOTOS/a_hitman's_hobby/hh_photo4.png)

Clicking through it you'll see an old archived newspaper dated to August 1, 1961. Scroll below and you'll see some highlighted yellow text.

![hh_photo5](THE_FORGOTTEN_FILES_PHOTOS/a_hitman's_hobby/hh_photo5.png)

"Tommy Gibbs is busy with a whole bunch of old and new watches sent in; He'll be all wrapped up for a while." This text didn't really give me anything. So I searched the other page of this newspaper and didn't find anything.

I decided to look at more archived newspapers of The Echo, and sorted them from 1960–1969.

![hh_photo6](THE_FORGOTTEN_FILES_PHOTOS/a_hitman's_hobby/hh_photo6.png)

There's also a cool thing about the site. Searching just plain Tommy Gibbs doesn't give you an accurate result.

![hh_photo7](THE_FORGOTTEN_FILES_PHOTOS/a_hitman's_hobby/hh_photo7.png)

When searching, it's better to add quotation marks to your searches.

![hh_photo8](THE_FORGOTTEN_FILES_PHOTOS/a_hitman's_hobby/hh_photo8.png)

After a bit of digging I found this phrase: "Tommy Gibbs has a hobby of watch making."

![hh_photo9](THE_FORGOTTEN_FILES_PHOTOS/a_hitman's_hobby/hh_photo9.png)
![hh_photo10](THE_FORGOTTEN_FILES_PHOTOS/a_hitman's_hobby/hh_photo10.png)

**Answer:** Watch Making

---

## 3. The Citrus Conspiracy

![cc_photo1](THE_FORGOTTEN_FILES_PHOTOS/the_citrus_conspiracy/cc_photo1.png)

**Task:** What was the club's phone number and what neighbouring business is still there today (use the format XXX-XXXX business)?

Searching lemon tree club dallas 1972 gave me broad results, but among them is an address, which narrows down the search.

![cc_photo2](THE_FORGOTTEN_FILES_PHOTOS/the_citrus_conspiracy/cc_photo2.png)

After searching the address I got a result.

![cc_photo3](THE_FORGOTTEN_FILES_PHOTOS/the_citrus_conspiracy/cc_photo3.png)
![cc_photo4](THE_FORGOTTEN_FILES_PHOTOS/the_citrus_conspiracy/cc_photo4.png)

I got a number. Now all I had to do was search for a nearby place.

Since this is the same newspaper archiving site as the last challenge, I also did the quoting search thing.

Since the address is 4305-A Lemmon I decided to start searching it starting with 4300 and increment it by 1 to see if there was a business nearby.

**Attempt 1:**

![cc_photo5](THE_FORGOTTEN_FILES_PHOTOS/the_citrus_conspiracy/cc_photo5.png)

**Attempt 2:**

![cc_photo6](THE_FORGOTTEN_FILES_PHOTOS/the_citrus_conspiracy/cc_photo6.png)

**Attempt 3:**

![cc_photo7](THE_FORGOTTEN_FILES_PHOTOS/the_citrus_conspiracy/cc_photo7.png)

**Attempt 4:**

![cc_photo8](THE_FORGOTTEN_FILES_PHOTOS/the_citrus_conspiracy/cc_photo8.png)

**Attempt 5:**

![cc_photo9](THE_FORGOTTEN_FILES_PHOTOS/the_citrus_conspiracy/cc_photo9.png)

I found one! I checked the newspaper and saw that the address near it was Kentucky Fried Chicken (KFC).

![cc_photo10](THE_FORGOTTEN_FILES_PHOTOS/the_citrus_conspiracy/cc_photo10.png)
![cc_photo11](THE_FORGOTTEN_FILES_PHOTOS/the_citrus_conspiracy/cc_photo11.png)

**Answer:** 526-1190 KFC

---

## 4. Beyond the Fence

![bf_photo1](THE_FORGOTTEN_FILES_PHOTOS/beyond_the_fence/bf_photo1.png)

**Task:** What are the coordinates of the former gunnery position and what was the name of the sea-plane base (use decimal degrees to 3 decimal places and add the base name after i.e. "51.513, -0.219 Harrow")?

The first thing I did was check the locations in google map. First I checked for Lobnitz, turns out it's in Germany but my initial search doesn't match the map.

![bf_photo2](THE_FORGOTTEN_FILES_PHOTOS/beyond_the_fence/bf_photo2.png)

But it's not the only Lobnitz in Germany, so one by one I checked them all.

![bf_photo3](THE_FORGOTTEN_FILES_PHOTOS/beyond_the_fence/bf_photo3.png)
![bf_photo4](THE_FORGOTTEN_FILES_PHOTOS/beyond_the_fence/bf_photo4.png)
![bf_photo5](THE_FORGOTTEN_FILES_PHOTOS/beyond_the_fence/bf_photo5.png)

Finally a match to the map!

Now all I had to do was search for the spots marked in the hand-drawn map.

First I decided to look for the seaplane base.

![bf_photo6](THE_FORGOTTEN_FILES_PHOTOS/beyond_the_fence/bf_photo6.png)

Just looking at the map, the sea plane base is near prestz. Now looking to the google map the nearest point in prestz (preetz) is kramerhof, since it is near the water.

![bf_photo7](THE_FORGOTTEN_FILES_PHOTOS/beyond_the_fence/bf_photo7.png)

Next thing I did was scan the area for anything military base.

After a few minutes I managed to find one.

![bf_photo8](THE_FORGOTTEN_FILES_PHOTOS/beyond_the_fence/bf_photo8.png)
![bf_photo9](THE_FORGOTTEN_FILES_PHOTOS/beyond_the_fence/bf_photo9.png)

Now that it's done, I started to look for the gun position in the western shore part.

Now looking at the map the only point where it matches the spot is Wustrow.

![bf_photo10](THE_FORGOTTEN_FILES_PHOTOS/beyond_the_fence/bf_photo10.png)
![bf_photo11](THE_FORGOTTEN_FILES_PHOTOS/beyond_the_fence/bf_photo11.png)

I started to scan the area. It took me a long while but I managed to see a bunker at Wustrow, near the shore.

![bf_photo12](THE_FORGOTTEN_FILES_PHOTOS/beyond_the_fence/bf_photo12.png)
![bf_photo13](THE_FORGOTTEN_FILES_PHOTOS/beyond_the_fence/bf_photo13.png)

Now all I had to do was copy the coordinates.

![bf_photo14](THE_FORGOTTEN_FILES_PHOTOS/beyond_the_fence/bf_photo14.png)

**Answer:** 54.361, 12.396 Parow

---

## 5. Slaughter and Salvation

![ss_photo1](THE_FORGOTTEN_FILES_PHOTOS/slaughter_and_salvation/ss_photo1.png)

**Task:** How much (to the nearest dollar) did the modern church cost to build?

The first thing that I did, of course, was search for the location in google maps, and scan the place.

After putting in minutes to hours just finding the exact spot in the map, I found out that the battlefield is actually quite far from the mountain.

![ss_photo2](THE_FORGOTTEN_FILES_PHOTOS/slaughter_and_salvation/ss_photo2.png)

At this point I changed strategy, instead of trying the exact spot, I decided to just look for the nearest church in Cedar Mountain Battlefield.

Crooked Run Church and Cedar Run Baptist Church

![ss_photo3](THE_FORGOTTEN_FILES_PHOTOS/slaughter_and_salvation/ss_photo3.png)

I searched for the church's history. I started with Crooked Run Church.

![ss_photo4](THE_FORGOTTEN_FILES_PHOTOS/slaughter_and_salvation/ss_photo4.png)
![ss_photo5](THE_FORGOTTEN_FILES_PHOTOS/slaughter_and_salvation/ss_photo5.png)

This wasn't the answer since the church was destroyed by fire in 1910.

Next is Cedar Run Baptist.

![ss_photo6](THE_FORGOTTEN_FILES_PHOTOS/slaughter_and_salvation/ss_photo6.png)
![ss_photo7](THE_FORGOTTEN_FILES_PHOTOS/slaughter_and_salvation/ss_photo7.png)

And this is the correct answer, it stood in the midst of the Battle of Cedar Mountain in August of 1862, and the construction cost is $1,450.00.

![ss_photo8](THE_FORGOTTEN_FILES_PHOTOS/slaughter_and_salvation/ss_photo8.png)

**Answer:** 1450

---

## Conclusion

Compared to my first write-up, these five challenges pushed me a lot further into the "wrong turn before the right one" side of OSINT. Cases like Beyond the Fence and Slaughter and Salvation weren't solved by a single clean search; they took hours of scanning maps, checking multiple candidate locations, and ruling out answers that seemed right until they weren't (Crooked Run Church looked promising until its history disproved it). Even the more straightforward cases, like The Citrus Conspiracy, only came together after several incremented guesses at nearby addresses.

This whole set was a lot more fun than the first one, and I'm hoping to write up more of these soon.
