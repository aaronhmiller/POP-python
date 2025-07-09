# POP
Proof of Pipeline for Python

Look in the workflows area...that's where the *real action* is (for we DevSecOps folks!)

## Usage
1. Increment the Version in the text at the bottom of this page (yes, yes, if this were a real flow, this would be an actual release tag, but pretend with me for the sake of an easy to showoff demo. kthxbye)
2. Commit the change (yes, yes again...directly to main...if this were real, you'd do this to a patch branch & from a PR AND you would have it reviewed by a person other than you, but let's take a shortcut...again, for the sake of an expedient demo. heheheh 😈)
3. The commit kicks off your workflows, so FINALLY we see what we came here for...from the repo's main area, select the "flows running" icon indicator and you should see three order independent flows:
   - Python (Latest)
   - Chainguarded Python

The scan results of each depend on the mix of CVEs in the actual images at the time of your run. So we have [that going for us. Which is nice.](https://youtu.be/X48G7Y0VWW4?feature=shared&t=60)

They will NOT promote any image with CRITICAL CVE(s). And by design, HIGHs are not JIRA-fied if there are criticals, because we assume that by the time the CRIT(S) are resolved, the mix of HIGHs will likely have changed and there are enough JIRAs out there already to keep us all busy for millenia 😬. MEDIUMs and LOWs are counted, but not expected to be acted upon. Just keepin' it real folks.

## What it should look something like
Handy [dandy video](https://share.cleanshot.com/GvThjHwv) for y'all who want to try this yourself. PRs welcome too!

## Versions
0.0.1g (honoring & paraphrasing [JWZ](https://www.jwz.org/) who said something once like "quality is job 1.1a")
