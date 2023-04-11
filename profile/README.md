## A GH org to test migration into Enterprise Cloud

Fork or clone repos from your GitHub orgs to test what happens when this org is migrated into Enterprise. I'll reach out to Marcus Nedelmann at NWFSC IT on Monday and let him know we want to try migrating this org in. NW has spare licenses right now so should be fine if you aren't on Enterprise yet and don't have one. Hopefully we can do a trial migrate by the end of the week.

* No non-NOAA collaborators for now since we don't want to eat up licenses
* Repos that do less common things, like used to post to Posit Connect or have unusual GitHub Actions are good
* Create projects or issues

## Repos on here now

* nmfs-test-migrate.github.io a Jekyll based page with lots of dependencies
* rCAX GitHub action builds a pkgdown page
* VRData nothing that special but I made it private so we can test private GitHub pages which is a new thing with Enterprise.

## Things that are likely to break

Per 4/10/23 discussion with GH Enterprise reps, nothing should break unless there are restrictions in place at the Enterprise level.

* ~~Fork relationships do not presist https://docs.github.com/en/migrations/using-ghe-migrator/exporting-migration-data-from-githubcom~~
* ~~Project boards are not migrated but everything else is~~

## Migration steps

Per 4/10/23 discussion with GH Enterprise reps

1. An Enterprise admin navigates to the page with the orgs listed
2. Clicks the "Invite" organization and pastes in the URL
3. The owner of the org will get an email (or notification) and selects "confirm" or "transfer"
4. That's it.

* ~~First use the backup.sh script (in GGT G-Drive) to make the migration archive. Download the archive and share with GHEC admin~~
  * ~~https://docs.github.com/en/rest/migrations/orgs?apiVersion=2022-11-28~~
  * ~~https://docs.github.com/en/migrations/using-ghe-migrator/exporting-migration-data-from-githubcom~~
* ~~Next a GHEC admin does the migration~~
  * ~~https://docs.github.com/en/migrations/using-ghe-migrator/preparing-to-migrate-data-to-github-enterprise-server~~
