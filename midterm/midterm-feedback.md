# Midterm Feedback

## Overall Score: 
45 / 50

This was well done.  The work at the end, putting the patient scores together was a little bit clunky with val=1 and length=335.  You could have just looped through the list using a for loop or at least calculated len(temp).


## Part 1: Creating a JSON Rules File
Comments - Nice work.  The only potential area I see that might be an issue is with FiO2 and knowing when to use which branch.  What range of FiO2 values dictate that.  I assume I'll find that logic in one of your functions.  (-1)

## Part 2: Functions to evaluate rules
Comments - I see how putting a lot of the rule calculations in one function like this might have seemed like a more efficient way to solve it.  However, you still have a lot of repeat code (for each rule) and that having a single function with all of these parts makes it harder to test individual pieces. (-1)

Also, your organ failure rules should have been in the JSON file and not in the code.  (-1)

With your fio2_score processor, I think you have a flaw in your logic.  There's nothing to select which score should be returned - the one based on pao2 or aa_gradient.  It won't work the way you expect it all the time.  (-1)

## Part 3: Put it all together
Comments - Nice work.  The only piece that should be corrected here is the fio2 range here rather than in the JSON.  I already took off one point for that above.


## Part 4: Accessing and processing the patient file
Comments - This generally looks like it works, but I wasn't able to verify it because there were some other errors in your code.  Generally nice work, though.  (-1)

I also also looking for the final comparison, but your code wouldn't run end-to-end.  (-1)