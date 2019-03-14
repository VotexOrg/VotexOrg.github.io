# VotexOrg.github.io

Votex is a voting system designed to create end-to-end voter-verifiable paper ballots. Votex supports alternative voting methods including ranked choice and score voting as well as conventional first-past-the-post voting.

Votex is built around the procedure below.

( [This app](https://votexorg.github.io/) can be used to create ballots, as described in steps 2 and 3. )


**1**

The administrator (or committee of administrators) compiles a voter roll.


**2**

**a.** The administrator uses an offline computer to generate a pair of unique random codes for each voter, a ballot code and an ownership code.
* The ballot code certifies that the ballot is authentic.
* The ownership code can be used to prove ownership of a ballot code if a ballot is maliciously intercepted before it is recorded.

**b.** The administrator prints out the list of valid code pairs and archives the papers in a secure locked box, to be opened after the voting deadline.


**3**

**a.** The administrator prints out ballots, each with a unique ballot code printed on the bottom.

**b.** For each ballot, administrators print a unique code page containing the corresponding ballot code and ownership code.


**4**

The ballot-generating computer is placed in an offline safe for auditing if necessary.


**5**

**a.** The ballots and code pages are paired within sealed envelopes.

**b.** The envelopes are shuffled to ensure secrecy.

**c.** The envelopes are distributed, either by mail or in person at polling stations.

**6**

**a.** Voters fill out the enclosed ballot. Or, if election rules allow it, voters may print out a new ballot (using their ballot code), adding write-in candidates if they wish.

**b.** Voters return the ballots by mail or in person.

**c.** Voters retain their code page if they want to confirm their vote later.


**7**

**a.** Ballots are scanned at polling stations and the paper is archived for auditing.

**b.** The scanned images are sent to a central server, which interprets the votes.


**8**

**a.** After the voting deadline, the administrators open the locked vault and scans the ballot codes into a database.

**b.** The scanned votes are filtered against the database of valid codes.

**c.** Valid votes are published as an ordered list starting at vote 1.  

**d.** Each vote also includes a running total of the score. For conventional voting and score voting, the cumulative score after vote (n) is a function of vote (n) and the cumulative score after vote (n-1). This allows decentralized auditors to confirm the tally.


**9**

Voters can enter their ballot code online and receive a link to the corresponding vote number. This allows voters to verify that their vote was recorded correctly.


**10**

The administrator certifies the result at a certification date.
