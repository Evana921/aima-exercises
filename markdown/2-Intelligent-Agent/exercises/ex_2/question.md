Let us examine the rationality of various
vacuum-cleaner agent functions.<br>
1.  Show that the simple vacuum-cleaner agent function described in
    Figure <a class="insideBookFigRef" target="_blank" href="https://aimacode.github.io/aima-exercises/figures/vacuum-agent-function-table.png">vacuum-agent-function-table</a> is indeed
    rational under the assumptions listed on page <a class="pageRef" title="" href="#">vacuum-rationality-page</a><br>

   

This agent is rational because:

    It always cleans a dirty square when it sees one (achieving the cleaning goal).
    It moves to check the other square when the current one is clean (avoiding being idle).
    It works well under the assumptions:
        There are only two squares (A and B).

 The vacuum looks at where it is and what it sees:

    If it’s at A and the square is dirty → Suck.
    If it’s at A and the square is clean → Move Right to check the next square.
    If it’s at B and the square is dirty → Suck.
    If it’s at B and the square is clean → Move Left to check the other square.

2.  Describe a rational agent function for the case in which each
    movement costs one point. Does the corresponding agent program
    require internal state?<br>

3.  Discuss possible agent designs for the cases in which clean squares
    can become dirty and the geography of the environment is unknown.
    Does it make sense for the agent to learn from its experience in
    these cases? If so, what should it learn? If not, why not?<br>
