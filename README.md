# MongoDB Aggregation Pipeline Bug

This repository demonstrates a common error in MongoDB aggregation pipelines:  incorrect use of the `$group` stage leading to inaccurate results.

The `bug.js` file contains the erroneous code. The `bugSolution.js` file provides the corrected code.

## Bug Description

The provided aggregation pipeline attempts to group documents, count occurrences of each group, sort by count, and limit the results.  Due to a logic error in the `$group` stage, the grouping and counting are inaccurate.  This results in an incorrect output when querying the collection.

## Solution

The `bugSolution.js` file shows the corrected aggregation pipeline. The issue is identified and resolved by ensuring the correct field is used for grouping and counting, resulting in the accurate results.