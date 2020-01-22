# flixster
# Flix

Flix is an app that allows users to browse movies from the [The Movie Database API](http://docs.themoviedb.apiary.io/#).

📝 `NOTE - PASTE PART 2 SNIPPET HERE:` Paste the README template for part 2 of this assignment here at the top. This will show a history of your development process, which users stories you completed and how your app looked and functioned at each step.

---

## Flix Part 1

### User Stories

#### REQUIRED (10pts)
- [x] (2pts) User sees an app icon on the home screen and a styled launch screen.
- [x] (5pts) User can view and scroll through a list of movies now playing in theaters.
- [x] (3pts) User can view the movie poster image for each movie.

#### BONUS
- [ ] (2pt) User can view the app on various device sizes and orientations.
- [ ] (1pt) Run your app on a real device.

### App Walkthough GIF

<img src="http://g.recordit.co/xtUtSTZRpV.gif" width=250> <img src="http://g.recordit.co/UuLWGEJ9oJ.gif" width=250><br>


### Notes

Errors I faced: 
  - SIGABRT Error 
  - Black screen after launching
  - Error that my "TableViewController" and "NavigationController is unreachable because it has no entry points and no runtime access. 
  - Could not print to console view
  
How I fixed these errors:
  - Realized I had to make a screen "is Initial View Controller"
  - Fixed Outlets because one label was used as the same outlet twice
  - Forgot to remove a line of code that was changed in the video walkthrough so there were two contradictory lines
  - Used Shift + Command + C to enable console view, because it was disabled on my mac

My notes:
- Learning Goal for Flix part 1 -> Implement Scrolling
- AppDelegate.swift : runs first time when app launches
- ViewController : screen, both collection of views and logic
- main.storyboard : where views are designed; arrow indicates first screen
- alpha : transparency
- Asset folder : add images
- Use Media Library to add images to screen (click Object Library and it is the next tab)
    - a Media Library image and an image view is the same, except the media library image auto-resizes
- Shift + Command + C shows console view
- var Movies [[String:Any]]() // Creation of an array of dictionaries; " () " indicates creation
- download array of movies and variable
- Casting as! String tells you type 

Table View Recipe:
1. Add parameters : UITableViewDataSource and UITableViewDelegate
2. Add outlets
3. Change the 2 lines to self
4. Add those 2 functions on the bottom
5. Implement count, cell creation, and reload data


