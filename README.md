# Beyond the Repository BagIt Profile
### Under active development

## Current Status
Draft for discussion

## Notes
For our recommended and searchable fields, I illustrate a couple possible approaches. Neither
of these results in an error from the profile validation component of the Python-based reference validator on the
[Bagit Profiles GitHub](https://github.com/bagit-profiles/bagit-profiles-validator).

The first approach uses an extension object, `BtR-Extensions`, in the `BagIt-Profile-Info` object
to enumerate recommended and searchable tags.

The second approach adds `recommended` and `capabitilies` properties to the tag properties objects in
the `Bag-Info` object. In this case, I made `searchable` a capability, with an eye toward the possibility of
other capabilities in the future.

For the nuanced cases with "optional/recommended*", I added a `description` property to the applicable
tag properties objects. This also caused no profile validation issues.

We will need to discuss these "adjustments" with the BagIt Profiles folks, if we'd like to see some/all of
these properties supported in the future.

We will also need to give some more thought to which organization will act as promulgator of this profile and who 
will act as contact.


