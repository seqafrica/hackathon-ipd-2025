# SeqAfrica Hackathon at IPD Feb 2025

This repo holds instruction, notes, links, etc. for the SeqAfrica Hackathon
at IPD in February 2025.


### What will we do?

The idea of a hackathon is that a group of developers - or in our case:
bioinformaticians - get together and build something in a limited time.

We will have a day and a half (17 Feb and the afternoon of 19 Feb) to work
on this.

We have set no hard deliverables, but have picked two themes:

 1. **Democratizing Analysis**: make bioinformatics analyses more accessible
 to end users

 2. **Harmonizing AMR Detection**: building on the work done by PH4AGE, use,
 improve or extend [hAMRonization](https://www.biorxiv.org/content/10.1101/2024.03.07.583950v1)
 ([GitHub repo](https://github.com/pha4ge/hAMRonization))

Ideally, the two themes come together around the "SeqAfrica sentinel site
ONT laptops" that we are currently piloting.  I would summarise the goal as:

_Provide the sentinel site ONT laptop users with an easy to use system that
produces clear, comprehensive, reliable and actionable analyses of their
bacterial isolates, in particular with respect to AMR_.

More practically you could think of:

 * Bringing together the "Big Three" (ResFinder, AMRFinderPlus, RGI) in a
   single harmonized workflow
 * A workflow to produce a phylogenetic tree from a local collection of
   sequenced isolates _without any need to "descend to the command-line"_
   * Ideally: annotated with sequences type, AMR, etc
   * Better yet: with added references based on location, time, ST, etc
   * ...
 * Producing analysis reports (paper or interactive) that can be shared
   with the "real" end users of our work: clinicians, PH officials, etc.
 * ...

Constraints?

 * Laptops will be deployed in locations with limited internet connectivity,
   so the solution should work with little or no network access
 * We intend to build this on top of EPI2ME, which can run locally and
   "in-cloud"; ONT are willing to assist with the second
 * The laptops run recent Ubuntu versions (22.04, 24.04), so this is our
   target platform

And of course: we want to have _at least working demos_ at the end of Day 2!


### How do I prepare?

First off, **please let me know (through email) your GitHub handle/username**
so I can add you to the SeqAfrica GitHub.

Please come with your own laptop, with **EPI2ME Desktop** installed.
Installation instructions are at <https://labs.epi2me.io/epi2me-docs/installation/>.

You may want to also have a separate Nextflow installation for experimentation
(instructions [here](https://www.nextflow.io/docs/latest/install.html), but
note that EPI2ME comes with a (slightly outdated) built-in Nextflow.

> **In case of issues**
>
> On Ubuntu 24.10 (and possibly 24.04, needs testing), you will likely have
> issues starting and/or configuring EPI2ME Desktop.  I have a workaround that
> I'll add to [this document](https://github.com/orgs/seqafrica/discussions/2).
>
> A separate issue (probably only on Ubuntu 24.10, but possibly also when you
> use "rootless Docker"): <https://github.com/epi2me-labs/wf-basecalling/issues/65>.
>
> If you encounter any other issue, please just submit them or start a discussion
> in this SeqAfrica repository, that's what it's for!

It will be good to familiarise yourself somethat with EPI2ME and/or Nextflow,
for instance by running the "Bacterial Genomes" workflow from EPI2ME Desktop
and taking a look in its GitHub repo: <https://github.com/epi2me-labs/wf-bacterial-genomes>.

Note in the README in that repository that you can also run the workflow directly
from Nextflow.  All EPI2ME workflows are under [epi2me-labs on GitHub](https://github.com/epi2me-labs).

**Looking forward to seeing you all in a week!**

