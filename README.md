# experiment-cardano-node-gh-actions
Trying to execute cardano node as part of github actions.

# Issue: First run is not enough to cache the status of the blockchain
so I created my owon fork of the action.
lowered the threshold to sync to 90%
will let it run.
once it actually caches something,
I'll go back and change it again.

# after days of fight with this what do I know now?
- the key is to stop the action with the wait-and-sync.sh script in a timeout.
- for some reason, sometimes it doesn't take the latest cache... it keeps finding the 70% one.
I could:
start a new, now only with the experiment. and modify the wait-and-sync file only and see how it goes. see if it works.

