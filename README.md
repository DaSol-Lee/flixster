# flixster
# Flix

Flix is an app that allows users to browse movies from the [The Movie Database API](http://docs.themoviedb.apiary.io/#).

## Flix Part 2

### User Stories

#### REQUIRED (10pts)
- [x] (5pts) User can tap a cell to see more details about a particular movie.
- [x] (5pts) User can tap a tab bar button to view a grid layout of Movie Posters using a CollectionView.

#### BONUS
- [ ] (2pts) User can tap a poster in the collection view to see a detail screen of that movie.
- [ ] (2pts) In the detail view, when the user taps the poster, a new screen is presented modally where they can view the trailer.

### App Walkthough GIF

<img src="http://g.recordit.co/Jo7BBgQNW2.gif" width=250><br>

### Notes

Errors I faced:
  - In the Collection View Setup, my Poster Views displayed small squares instead of the normal sized poster as shown in the video, although I adjusted the size manually on the main.storyboard
  - Created an outlet with the UIView instead of the UIImageView
  
  
How I fixed these errors:
  - Set the estimate size in collection view on the main storyboard to none instead of the its current set to automatic, which was probably why the cells were adjusting their size dynamically (from CodePath Discussions)
  - Deleted the outlet and dragged the correct one


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


