# Lesson 03 - Strings

# Exercise: Making a List
Lists are great. Here are some constants describing some of the things you’ve learned about strings so far:

```swift
let constants = "Declaring string constants"
let unicode = "Unicode characters (😎)"
let combining = "Combining strings using +"
let interpolation = "String interpolation (aka Fill in the Blanks)"
let escaping = "Escape characters for \"special powers\""
let newline = "Making new lines"
```

## Experiment
Make a new string constant that is a list of the things you’ve learned, with each entry on a new line. Make sure you add the result to the playground page so that you can see the list properly.

```swift
let list = "\(constants)\n\(unicode)\n\(combining)\n\(interpolation)\n\(escaping)\n\(newline)"

// "Declaring string constants\nUnicode characters (😎)\nCombining strings using +\nString interpolation (aka Fill in the Blanks)\nEscape characters for "special powers"\nMaking new lines"
```

# Exercise: A Restaurant

```swift
let customerOrderOne = "fish"
let customerOrderTwo = "risotto"
let customerOrderThree = "soup"

let serverResponseToTableOne = "Let me make sure I've got this right: \(customerOrderOne), \(customerOrderTwo), and \(customerOrderThree). Is that everything?"

let tableOneResponse = "Yes, thank you!"
```

## Later that Day:
Three other guests enter and place their orders:

```swift
let customerOrderFour = "돌솥비빔밥"
let customerOrderFive = "Pasztecik szczeciński"
let customerOrderSix = "小笼包"
```

The server speaks all of these languages and confidently repeats the orders back to the group.

## Exercise
Make sure the server repeats the order correctly without copying and pasting or retyping any of the orders.

```swift
let serverResponseToTableTwo = "Let me make sure I've got this right: \(customerOrderFour), \(customerOrderFive), and \(customerOrderSix). Is that correct?"

let tableTwoResponse = "Perfect, merci bien."
```
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

# Exercise: Displaying Values

You may recall from an earlier playground an exercise that involved calculating the space remaining on an iPhone. You had the following information:

* The capacity of an iPhone is measured in gigabytes (GB). The iPhone in question has 8GB of storage.
* A gigabyte is about 1,000 megabytes (MB)
* The phone already has 3GB of stuff on it
* One minute of video takes 150MB of space

## Exercise
Create a string that tells the user how many minutes of video they can store on the phone. You'll first need to perform the calculation steps, then use string interpolation to display the answer - which should look like this:
```You can record XXX more minutes of video.```

```swift
// All Calculations in Megabytes

let usedCapacity = 3
let phoneCapacity = 8 - usedCapacity
let capacityMB = phoneCapacity * 1000
let oneMinuteVideo = 150
let totalVideoMinutes = capacityMB / oneMinuteVideo
print("You can record \(totalVideoMinutes) more minutes of video.")

// Output: You can record 33 more minutes of Video
```
