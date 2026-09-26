# weeklyetfs-x-poster

Posts scheduled WeeklyETFs posts to X as @WeeklyETFs.

Posts are added by the queue tool at weeklyetfs.com/x-queue. Every 30 minutes a cron-job.org timer
starts the "Post to X" workflow, which posts anything that is due and moves it to `posted/`.
Anything X rejects lands in `failed/` with the reason.

The script checks which account the keys belong to before posting and stops if it isn't @WeeklyETFs.
