# Jenkins Multi Master Setup with AWS EC2 and EFS

1. Create 2 EC2 instances
2. Create EFS
3. Mount EFS on /var/lib/jenkins or $JENKINS_HOME path
4. Create cron job with the jenkins_reload.sh set to run every minute
5. Setup HAproxy with jenkins 1 as Active and jenkins 2 as standby configurations


### Good  HA solution for jenkins OSS but if job is running on active node and the node goes down job is lost.

# Jenkins Backup and Restore

Follow the steps in **Jenkins-backup-restore.docx** to backup and restore jenkins 
