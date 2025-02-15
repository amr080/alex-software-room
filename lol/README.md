## Salt Typhoon 

1. Primary Analytics URL Pattern:


```plaintext
bam.nr-data.net/jserrors/1/NRBR-0fefdffb87aeaab02ff
```

2. Full URLs with suspicious parameters:


```plaintext
bam.nr-data.net/jserrors/1/NRBR-0fefdffb87aeaab02ff?a=90967276&v=1.277.0&to=NFdXMkMDD0sFB0ZeXw0deDByTSBKEA1RW1UQcVoIRRAOVAgBQBh0BkZUD10R&rst=1017793&ck=0&s=6138efbd9eeda429&ref=https://www.informit.com/articles/article.aspx&ptid=a9bb344575ff1790
```

3. Secondary Analytics URL Pattern:


```plaintext
bam.nr-data.net/browser/blobs?browser_monitoring_key=NRBR-0fefdffb87aeaab02ff
```

4. Suspicious Parameters Found:


- `harvestId=6138efbd9eeda429`
- `trace.originTimestamp=1736322713234`
- `entityGuid=MTMyMjQ4MHxCUk9XU0VSfEFQUExJQ0FUSU9OfDkwOTY3Mjk0`


5. Redirect Chain:


```plaintext
http://www.informit.com/articles/article.aspx?p=366891&seqNum=2
-> addTo.aspx?p=feab3e8a-c2e6-49f9-8873-8d0d83ced9e1&e=bc4c912f-c86a-473f-98ba-71ac4aad9e5c
```

6. Mail Server Involved:


```plaintext
mailwash14.pair.com (66.39.2.55)
```


### New Relic
bam, browser application monitoring
Endpoints:


rbs2.com

https://bam.nr-data.net/browser/blobs      # Browser session tracking
https://bam.nr-data.net/jserrors/1/        # JavaScript error reporting 
https://bam.nr-data.net/events/1/          # Event tracking
https://bam.nr-data.net/ins/1/             # Instrumentation data

https://bam.nr-data.net/
{"description":"GET / not found","error":"tigertonic.NotFound"}


/browser/blobs
/jserrors/1/
/events/1/
/ins/1/

Key parameters:
browser_monitoring_key: NRBR-0fefdffb87aeaab02ff
app_id: 90967276
agentVersion: 1.277.0
session: 6138efbd9eeda429
entityGuid: MTMyMjQ4MHxCUk9XU0VSfEFQUExJQ0FUSU9OfDkwOTY3Mjk0


The website (informit.com) was trying to send analytics data to New Relic's servers at bam.nr-data.net but failed due to an internet connectivity issue.
