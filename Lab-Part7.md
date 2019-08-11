# Verify that your data migration completed successfully

After the migration is complete, connect to SQL Workbench and your Redshift cluster and verify counts in the following tables

Query | Count
---- | ----
select count(*) from dim_person; | 7055276
select count(*) from dim_player; | 5157
select count(*) from dim_sport_location_seats; | 3565082
select count(*) from dim_sport_team;| 62
select count(*) from dim_sporting_event; | 1142
select count(*) from fact_sport_event_ticket_info; | 56530154

## Conclusion

You have completed the workshop.  In this workshop you have created a simulated on-premise Oracle source database and used AWS SCT to convert your schema and migrate your data.

## Delete all resources

Make sure you delete the Replication instance. Once the replication instance is deleted you should be able to delete the CloudFormation stack, which will in turn delete all resources.

**Note: If you do not delete resources they will keep incurring charges.**

1.	Open the CloudFormation console at this [link](https://console.aws.amazon.com/cloudformation/home)

2.	Select the checkbox for the stack you created for this lab.

3.	Select Actions and Delete Stack.  Select Yes, Delete.  CloudFormation will delete all resources created.
