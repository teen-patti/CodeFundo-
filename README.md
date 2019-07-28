# CodeFundo-

What are we planning to build ?

So,basically in most of the colleges/educational institutions in India elections are conducted for the position of 
General Secretary in disciplines such as Academic affairs/Technical affairs/Cultural affairs/Sports affairs and many such. But, 
still the elections are held like we are in 20th century, all that old paper ballots and stamps. We propose a system through
which colleges/educational institutions or any other organisation can conduct elections for any position/appraisal/review/feedback form.

How does it work ?

There will be biometric setup at the entry of booth. After enrollment/employment number and biometric verification (fingerprint authentication),
the person will cast his vote in a system. A system (end to end encrypted) will accept his vote. Till this everything was so trivial, but 
our main focus is to ensure that the vote count should not be tampered. So for that, we are using the concept of hashing along with blockchain
mechanism to ensure that. Every user id i.e. enrollment/employment number will be hashed with a randomly generated hash function.
With an another hash function, the aadhar number will be hashed so that the details are safe. A database (based on blockchain mechanism) 
will be created. It will constitute the hashed id, hashed aadhar number and a column whether the time stamp of the voter(the time of vote or not. Let's say there are
X parties/people contesting in election, according to the number of eligible voters, for each party N different hash keys will be generated and stored.
The load will get balanced in this way, also with so many different (particulary X*N) vote countering columns, one cannot tamper the vote in favour of
his party as he will not be able to know which column corresponds to which party vote count. At last, all the X*N counters will be re-hashed to count the vote.
In this way, there will be no need to use paper ballots and time will also be saved as the vote count can be accessed as soon as the election ends.

How users can get started with the project?

Just upload the database of voters. And the system will automatically retrieve the aadhar data using biometric authentication from government databases.

What datasets are we using ? 

As such we will not have the access to any dataset whether it be aadhar number data provided by government or the voter database provided by the institute.
Its just like rest API, we will use the data without having access to whole system database so that private information doesn't get compromised.


