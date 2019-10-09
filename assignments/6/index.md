# Assignment 6: Implementation · React

Starting from the code we wrote together in [lecture](/lectures/6), add the following features.

# A “Play Again” Button

<figure markdown="1">
![Play Again](play-again.png){:width="309"}
<figcaption>
A screenshot of the game with the “Play Again” button.
</figcaption>
</figure>

The button must work by resetting the state of the React components, not by reload the page.

# Lizard 🦎 and Spock 🖖

Extend the game following the rules from [this The Big Bang Theory episode](https://bigbangtheory.fandom.com/wiki/Rock,_Paper,_Scissors,_Lizard,_Spock).

# Add an Explanation of Why Someone Won

With Lizard and Spock the game got too complicated, so a simple “Player 2 wins!” isn’t enough anymore. When the game is over, add an explanation, for example, “Lizard poisons Spock, so Player 2 wins!”

# Submission

**<small>⚠️</small>  Your assignment is submitted only when you submit the form below.**

<form method="POST" action="https://roboose.herokuapp.com/roboose/assignments" markdown="1">
<fieldset markdown="1">

<legend>Assignment</legend>

<input type="hidden" name="assignment" value="6">

<label>
**GitHub Identifier**  
<input type="text" name="github" required pattern="[A-Za-z0-9][A-Za-z0-9-]*[A-Za-z0-9]">  
</label>
<small>
For example, [`jhu-oose-example-student`](https://github.com/jhu-oose-example-student).  
Don’t include an `@` sign at the beginning—this isn’t a [mention](https://help.github.com/en/articles/basic-writing-and-formatting-syntax#mentioning-people-and-teams).  
GitHub identifiers **do not** start with `2019-student-`.  
</small>

<label>
**Commit Identifier**  
<input type="text" name="commit" required pattern="[0-9a-f]{40}">  
</label>
<small>
For example, [`48092726db45fd4bcde21e3712ac2d8e4a094797`](https://github.com/jhu-oose/www.jhu-oose.com/commit/48092726db45fd4bcde21e3712ac2d8e4a094797).  
Graders will look at the code base as of this commit.  
You may find the commit identifier on the commits page at `https://github.com/jhu-oose/{{site.course}}-student-<identifier>/commits/master`. Usually you want the most recent commit.  
</small>

</fieldset>

<fieldset markdown="1">

<legend markdown="1">Anonymous Feedback on [Lecture 6](/lectures/6)</legend>

**Confidence**  
<label>
<input type="radio" name="feedback[lecture][confidence]" value="decreased" required>
The lecture **decreased** my confidence in the material that was covered.
</label>  
<label>
<input type="radio" name="feedback[lecture][confidence]" value="no-effect" required>
The lecture **didn’t affect** my confidence in the material that was covered.
</label>  
<label>
<input type="radio" name="feedback[lecture][confidence]" value="increased" required>
The lecture **increased** my confidence in the material that was covered.
</label>

**Relevance**  
<label>
<input type="radio" name="feedback[lecture][relevance]" value="irrelevant" required>
The lecture covered material that seemed **irrelevant**.
</label>  
<label>
<input type="radio" name="feedback[lecture][relevance]" value="cant-tell" required>
The lecture covered material that I **can’t tell** whether is relevant or not.
</label>  
<label>
<input type="radio" name="feedback[lecture][relevance]" value="relevant" required>
The lecture covered material that I can tell is **relevant**.
</label>

**Difficulty**  
<label>
<input type="radio" name="feedback[lecture][difficulty]" value="too-difficult" required>
The lecture was **too difficult** and I had trouble following.
</label>  
<label>
<input type="radio" name="feedback[lecture][difficulty]" value="right-level" required>
The lecture was **at the right level** of difficulty for me.
</label>  
<label>
<input type="radio" name="feedback[lecture][difficulty]" value="too-easy" required>
The lecture was **too easy** and I got bored.
</label>

**Pace**  
<label>
<input type="radio" name="feedback[lecture][pace]" value="too-fast" required>
The lecture was **too fast** and I had trouble following.
</label>  
<label>
<input type="radio" name="feedback[lecture][pace]" value="right-pace" required>
The lecture was **at the right pace** for me.
</label>  
<label>
<input type="radio" name="feedback[lecture][pace]" value="too-slow" required>
The lecture was **too slow** and I got bored.
</label>

<label for="feedback--lecture--liked">
**At Least One Specific Thing That You Liked**
</label>
<textarea name="feedback[lecture][liked]" id="feedback--lecture--liked" required></textarea>

<label for="feedback--lecture--improved">
**At Least One Specific Thing That You Think Should Be Improved**
</label>
<textarea name="feedback[lecture][improved]" id="feedback--lecture--improved" required></textarea>

</fieldset>

<fieldset markdown="1">

<legend markdown="1">Anonymous Feedback on [Assignment 6](/assignments/6)</legend>

<label>
**Approximate Number of Hours Spent**  
<input type="number" name="feedback[assignment][hours]" min="1" max="100" required>
</label>

**Confidence**  
<label>
<input type="radio" name="feedback[assignment][confidence]" value="decreased" required>
The assignment **decreased** my confidence in the material that was covered.
</label>  
<label>
<input type="radio" name="feedback[assignment][confidence]" value="no-effect" required>
The assignment **didn’t affect** my confidence in the material that was covered.
</label>  
<label>
<input type="radio" name="feedback[assignment][confidence]" value="increased" required>
The assignment **increased** my confidence in the material that was covered.
</label>

**Relevance**  
<label>
<input type="radio" name="feedback[assignment][relevance]" value="irrelevant" required>
The assignment covered material that seemed **irrelevant** or **didn’t connect well** with the lecture.
</label>  
<label>
<input type="radio" name="feedback[assignment][relevance]" value="cant-tell" required>
The assignment covered material that I **can’t tell** whether is relevant or not or whether it connects with the lecture or not.
</label>  
<label>
<input type="radio" name="feedback[assignment][relevance]" value="relevant" required>
The assignment covered material that I can tell is **relevant** and **connects well** with the lecture.
</label>

**Difficulty**  
<label>
<input type="radio" name="feedback[assignment][difficulty]" value="too-difficult" required>
The assignment was **too difficult** and I had trouble completing it.
</label>  
<label>
<input type="radio" name="feedback[assignment][difficulty]" value="right-level" required>
The assignment was **at the right level** of difficulty for me.
</label>  
<label>
<input type="radio" name="feedback[assignment][difficulty]" value="too-easy" required>
The assignment was **too easy** and I got bored.
</label>

**Load**  
<label>
<input type="radio" name="feedback[assignment][load]" value="too-much-work" required>
The assignment was **too much work** and I had trouble completing it.
</label>  
<label>
<input type="radio" name="feedback[assignment][load]" value="right-amount" required>
The assignment was **the right amount of work** for me.
</label>  
<label>
<input type="radio" name="feedback[assignment][load]" value="too-little-work" required>
The assignment was **too little work** and I got bored.
</label>

<label for="feedback--assignment--liked">
**At Least One Specific Thing That You Liked**
</label>
<textarea name="feedback[assignment][liked]" id="feedback--assignment--liked" required></textarea>

<label for="feedback--assignment--improved">
**At Least One Specific Thing That You Think Should Be Improved**
</label>
<textarea name="feedback[assignment][improved]" id="feedback--assignment--improved" required></textarea>

</fieldset>

**<small>⚠️</small>  Don’t submit this form multiple times.**

<button>Submit</button>

</form>

If you run into problems, send an email to <assignment-submission@jhu-oose.com>. Include the information about the submission: your GitHub Identifier and the Commit Identifier. Don’t include any information about the feedback—it’s anonymous.
