# iOS9 and iOS12 Demo Day

## Requirements

1. Fork and clone the repository
2. **Add your presentation content**
    1. Slide deck (4 required slides)
    2. Links
    3. Answer all questions 
    4. YouTube demo video (1-2 min max)
3. Polish your Github Code repository
    1. Add screenshots and an overview to your GitHub Code Repository
    2. You should make that repository the "Public Portfolio" for your project
    3. Look at [John Sundell's Splash project](https://github.com/JohnSundell/Splash) for inspiration (code, images, GIFs)
4. Create a pull request (PR) and **tag your TL and Instructor**

## Links

* Github Code: `<https://github.com/alexnrhodes/FowlWeather>`
* Github Proposal: `https://github.com/alexnrhodes/ios-build-sprint-project-proposal`
* Trello/Github Project Kanban: `<https://trello.com/b/03n4pMi0/fowlweather>`
* Test Flight Signup (Recommended): `<https://testflight.apple.com/join/Uj050Pom>`

## Hero Image

`<Post one screenshot in an iPhone Simulator frame or an iPhone 11 Pro render using placeit.com>`

## Questions (Answer indented below)

1. What was your favorite feature to implement? Why?

`Definitely the search feature.  It took quite a bit of logic to minimalize the backend code.`

2. What was your #1 obstacle or bug that you fixed? How did you fix it?

`Our largest bug was with not taking into account ALL of the different weather edge cases.`
  
3. Share a chunk of code (or file) you're proud of and explain why.
```
    ` func fetchCLLocationFromSearch(with searchTerm: String) {
           geocoder.geocodeAddressString(searchTerm) { (placeMarks, error) in
               if let error = error {
                   NSLog("Error getting CLLocation from searchTerm: \(searchTerm) with error:\(error)")
                   return
               }
               
               guard let placemark = placeMarks?.first,
                   let location = placemark.location else { return }
               self.searchedLocation = location
           }
       }
 ``` 
 `This one was cool because it was a new function I had never used before and it is extremely powerful`
 
4. What is your elevator pitch? (30 second description your Grandma or a 5-year old would understand)
    `Is you're dad constantly asking if it is going to rain today?` 
    `Are your eyes starting to hurt from all of the eye rolling at your dads tired jokes?`
    `Say no more.`
    `Introducing Fowl Weather!`
    `A place where your dad joke enthusiast can tell if it's going to rain and make those hard decisions like, whether or not they can wear their crocs!  All while getting fresh new dad joke material!`

5. What is your #1 feature?

`Dad joke generator.`
  
6. What are you future goals?

`Implement a detail view for the forcast.  Adding a weather map`

## Required Slides (Add your Keynote to your PR)

1. App Name / Team Slide
2. Elevator Pitch
3. Your #1 Feature (Customer facing — what can I do with your app?)
4. Future Goals

## Slide Requirements

1. 50 pt font minimum
2. Be concise — don't write sentences/paragraphs (put these in your slide notes for speaking)
3. 3-6 bullets maximum per slide
4. Do the squint test (can you read the text if you squint, if so, make the font bigger)
6. Images are always welcome
7. Do the Grandma Test (Would your Grandma understand you?)

### Optional Slides

1. Blooper: What's a funny bug or blooper? (screenshots/GIFs please)
2. Revenue Model: If the app was your sole source of income, how would you monetize it?

## Presentation Format

**7 minutes/team**

* 4 minute presentation (5 minute hard cap)
* 3 minutes of questions

We have ~12 teams presenting today — please practice your presentation with a timer (as a team), and make sure you fit within the time limit.

Plan on having one person present the slides and live demo. Please practice your presentation in front of a mirror or with your team 2-5 times. Have the app running and visible (Simulator or QuickTime) so you can quickly transition between slides and live demo.

* App Name / Team Slide (30 seconds)
* Elevator Pitch Slide (30 seconds)
* Your #1 Feature (30 seconds)
* Live Demo (2 minutes)
* Future Goals (30 seconds)
* Questions (3 minutes)
