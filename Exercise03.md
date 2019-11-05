# Exercise: Go! Fight! Win!

Many schools have “fight songs”: Students learn at least some portion of the words and then sing the songs together loudly at school events like sports games.

You’ve decided that your school’s fight song needs a rewrite. You want to edit the song in code so you don’t have to copy and paste as much while you work.

1. Edit the song to have more than a repeated refrain.
2. Edit the refrain to have actual words.
3. Edit the refrain to use the schoolName at least twice.
4. Test your work by changing the school name to a fictional school.

Use string interpolation in case you decide to sell your brilliant song to another school.

Note:
Use the show result button to view the results of your work.

```swift
let schoolName = "Macintosh High"
//Ouput:  Macintosh High

let refrain = "\(schoolName), we measure in bytes. \(schoolName), fight fight fight"
// Output: Macintosh High, we measure in bytes. Macintosh High, fight fight fight

let song = "\(refrain)\n\(refrain)"
// Output: Macintosh High, we measure in bytes. Macintosh High, fight fight fight\nMacintosh High, we measure in bytes. Macintosh High, fight fight fight
```
