> Author: Seojun Lee(Best Of the Best 13th digital forensic track)
# Cloudgoat-Scenario-Glue_privesc

Install Scenario
```python
./cloudgoat.py create glue_privesc
```

## Scenario Start(s)

Web address

## Scenario Goal(s)

Find a secret string stored in the ssm parameter store

## Summary

There is an environment that is implemented as shown in the schematic drawing below. Glue service manager will accidentally upload their access keys through the web page. The manager hurriedly deleted the key from s3, but does not recognize that the key was stored in the DB.

Find the manager's key and access the ssm parameter store with a vulnerable permission to find the parameter value named “flag”.