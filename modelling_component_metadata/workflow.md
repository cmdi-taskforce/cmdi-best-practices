## Workflow {#workflow}

When developing a profile for a resource type hosted in your centre’s repository,

1.  First specify the requirements (e.g. relevant information, compatibility with existing archive standards or formats commonly used for specific resource types).
    *   If you will be creating profiles for different resource types, a _modular approach_ is recommended, where you e.g. re-use one component for general information and/or a general collection component within all profiles.
2.  To find existing profiles and components on which your profile could be based, check the [CLARIN Component Registry](https://catalog.clarin.eu/ds/ComponentRegistry) and assess suitable candidates with the [CLARIN Curation Module](https://clarin.oeaw.ac.at/curate/), which provides a precomputed assessment of all public profiles. (You can sort the list of profile assessment by their VLO facet coverage, which, together with string-filtering on the profile name provides a useful prioritized preselected list of profiles to be inspected for suitability manually.) The [CLARIN SMC Browser](https://clarin.oeaw.ac.at/smc-browser/index.html) is also useful in evaluating profiles, components, elements and data categories used in CMDI metadata.
    *   Remember that you can also reuse an existing profile directly as is, you don’t need to create a new one, if an existing one covers all your needs.
    *   When considering components for re-use from different sources in one profile, make sure there are no overlaps, e.g. certain elements/concepts occur more than once.
    *   If you find that a general component needs to be revised, e.g. because an important value is missing from its closed vocabulary, it’s a good idea to contact the creator/owner of the component (or the maintainer of the Component Registry via [cmdi@clarin.eu](mailto:cmdi@clarin.eu)) and point out the problem before you simply improve a copy for your own profile. If the existing component really needs to be improved, then it’s better to create a new version of this component and deprecate the old one to avoid proliferation of components in the Component Registry.
3.  If necessary, edit the profile and any new components in your workspace until the profile satisfies the requirements set up in the beginning.
4.  To assess the private profile with the [CLARIN Curation Module](https://clarin.oeaw.ac.at/curate/), use the assessment form and enter the URL of the profile as provided by the Component Registry. This test will inform you of the basic metadata quality and the compatibility with the CLARIN infrastructure and it should be repeated after making any adjustments to the profile, e.g. regarding covered concepts.
    *   Should _you find that suboptimal scores seem to be due to some concepts used in your profile are not being recognized, review the current version of the_ [_facet definitions for the VLO_](https://github.com/clarin-eric/VLO/blob/master/vlo-commons/src/main/resources/facetConcepts.xml) _for further information and/or contact the_ _Helpdesk__._
5.  Publish the finalized profile with development status a.k.a. “as draft” (after publishing any new components).
6.  Before moving from development to production status for the profile, it is recommended to first generate CMDI records and let them be harvested and displayed by the VLO for a number of resources based on this profile, since a need for minor corrections or changes might occur. If you want to use the VLO Alpha instance for testing, please contact vlo@clarin.eu.
7.  Should corrections or updates be required for a profile in production state, the current version should be deprecated and the corrected version defined as successor. Further instructions on how to deprecate items and set successors can be found in the Component Registry Documentation[^1]. As deprecation of the profile used does not influence the CMDI score in the Curation Model or the ranking in the VLO, this will not cause problems for users of your profile.

[^1]: https://www.clarin.eu/content/component-registry-documentation