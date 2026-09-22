# Permissions Lab — Day 4

## Setup
- Created 3 users: alice, bob, carol
- Created a group `team`, added all three
- Created alice_private, bob_private (700, owned individually)
- Created shared_folder (770, owned by vikki:team)

## What broke
- shared_folder was inside ~/ (home directory), which was rwxr-x---
- This blocked alice/bob/carol from even entering the path, 
  even though shared_folder itself had correct permissions
- Fixed by moving shared_folder to /srv, which has open execute (x) 
  permission for everyone

## What I learned
- Permissions are checked at every folder in the path, not just the final one
- 700 = private (owner only), 770 = shared with group
- chown changes owner/group, chmod changes what they can do
- Confirmed team members can't access each other's private folders
