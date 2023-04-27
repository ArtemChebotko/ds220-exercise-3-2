<!-- TOP -->
<div class="top">
  <img class="scenario-academy-logo" src="https://datastax-academy.github.io/katapod-shared-assets/images/ds-academy-2023.svg" />
  <div class="scenario-title-section">
    <span class="scenario-title">Exercise 3.2: Using Counters in CQL</span>
    <span class="scenario-subtitle">ℹ️ For technical support, please contact us via <a href="mailto:academy@datastax.com">email</a>.</span>
  </div>
</div>


<!-- NAVIGATION -->
<div id="navigation-top" class="navigation-top">
 <a href='command:katapod.loadPage?[{"step":"intro"}]'
   class="btn btn-dark navigation-top-left">⬅️ Back
 </a>
<span class="step-count"> Step 1 of 4</span>
 <a href='command:katapod.loadPage?[{"step":"step2-cassandra"}]' 
    class="btn btn-dark navigation-top-right">Next ➡️
  </a>
</div>

<!-- CONTENT -->

<div class="step-title">Use case background</div>

You have been on a roll lately designing tables, and that hasn't gone unnoticed. Since no good deed goes unpunished, your team has unanimously agreed to let you tackle one of the trickier problems they encountered learning Cassandra.

The problem is with keeping track of the number of videos in a particular category. Whenever a tag is added to a video, a transaction is done which reads the number of videos for that video category, increments it by one, and updates it in the database. However, this technique is susceptible to race conditions. Cassandra is a distributed database that allows for concurrent, simultaneous operations, and it does not allow transactions. Your team has been stumped on how to get this functionality working correctly in Cassandra. Fortunately, you have just read up on the counter type and know that it is the perfect way to solve this problem.

The requirement itself is to be able to support a query that can retrieve the number of videos for a particular category, defined as a specific tag and year added. The query allows querying on a tag, and optionally, on a range for the added year.

<!-- NAVIGATION -->
<div id="navigation-bottom" class="navigation-bottom">
 <a href='command:katapod.loadPage?[{"step":"intro"}]'
   class="btn btn-dark navigation-bottom-left">⬅️ Back
 </a>
 <a href='command:katapod.loadPage?[{"step":"step2-cassandra"}]'
    class="btn btn-dark navigation-bottom-right">Next ➡️
  </a>
</div>
