
# Notes for [How to Get Your Release Through the Incubator - Justin Mclean, Class Software](https://www.youtube.com/watch?v=I0-lp1t9ee0&index=40&list=PLbzoR-pLrL6pLDCyPxByWQwYTL-JrF5Rp)

## Incubator vote process

* create a release candidate
* vote on dev ML(requires atleast 3 +1 and +1 > -1)
* vote on incubator ML(requires atleast 3 +1 and +1 > -1)

any of the vote fails then recreate a RC

## Top reasons for -1 vote

* binary in source release

* including Cat. X and Cat. B licenced software

* License or notice issue

* Copyright issue

* Missing header or header issue

* Contains encryption software


## Signing

release must be cryptographically signed and it's better to use an apache.org email

## Disclaimer

Optional but best to provide one, can be in README

## Tagging

provide tagging along with hash in vote email

## Licensing

 should be clear, consistent, and do not joke on licensing

*useful tools*

* rat

* [compliance rockes](http://clmpliance.rocks)

### types of files needs extra attention

* JS files

 * JS files may be minified and thus missing license
 * bundled softwares
 * license change between versions

* photos and images

* fonts. The license in the metadata may not be accurate, check the source

## License category

* Cat. A (can bundle and can depend on)
  
  Apache 2.0/1.1, 2/3 clause BSD(without advertising), MIT/X11, W3C, Unicode, CC copyright 
  only, WTF public license
  
* Cat. B (can't include in source release, restricted use)
  
  CCDL, EPL, MPL, CC-A
  
* Cat. X (can't be used)

  GPL, LGPL, CC non commercial, JSON, BSD 4 clause, Apache 1.0(may be ok)

## Reading materials

* [Legal questions](https://www.apache.org/legal/resolved)

* Incubator release process

  [release management](http://incubator.apache.org/guides/releasemanagement.html)
  
  [release](https://incubator.apache.org/guides/release.html)
  
* [Assembling license and notice how to](http://www.apache.org/dev/licensing-howto.html)

* [apache maturity model](http://community.apache.org/apache-way/apache-project-maturity-model.html)

* [legal mailing list archive](http://mail-archives.apache.org/mod_mbox/www-legal-discuss/)

* [legal jira](https://issues.apache.org/jira/browse/LEGAL)
