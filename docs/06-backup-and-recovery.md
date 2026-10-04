# Backup & Recovery

## Objective
Prove the service can be recovered—not merely backed up.

## Plan
Back up all data/configuration required by the deployment while protecting secrets appropriately. Maintain at least one copy separate from the live service.

## Recovery Exercise
1. Record the current service state.
2. Create a backup.
3. Restore into an isolated test location or recovery instance.
4. Start the recovered service.
5. Verify test records exist.
6. Document recovery time and any missing dependencies.

## Evidence
Capture backup metadata and successful restored test data, never real vault contents.

## Lesson
A backup is not trusted until restoration has been tested.
