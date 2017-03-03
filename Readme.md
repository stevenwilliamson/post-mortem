
# Post mortems and information availble on failures

## Public Cloud Platform Related Issues

### AWS Outage

S3 went down due to operator error, knock on effect for other services. Common theme recovery took longer
than expected.

* https://aws.amazon.com/message/41926/


### Xero AWS issues

* https://www.xero.com/blog/2016/11/bumps-in-the-road-and-what-were-doing-about-them/


### Joyent suffered an outage due to operator error

Incident involved Triton, Joyent, SmartOS, operator error

* https://www.joyent.com/blog/postmortem-for-outage-of-us-east-1-may-27-2014

## Instapaper outage due to Amazon RDS issue

Incident caused by software constraint that was unknown to engineering team. Been a hosted RDS service
recover options were constrained. Similar to the Gitlab issue testing complete restores and optomising recover from worst case (complete loss) incidents would have resulted in faster recovery. Or at least helped highlight how long recover is really likely to take.

* https://medium.com/making-instapaper/instapaper-outage-cause-recovery-3c32a7e9cc5f#.b205ft8vs

## Dataloss Incidents

### Gitlab suffered dataloss and prolonged incident due to lack of working backups.

Incident involves operator error, postgresql, replication, and recovery issues (untested restores)

* https://docs.google.com/document/d/1GCK53YDcBWQveod9kfzW-VCxIABGiryG7_z_6jHdVik/pub
