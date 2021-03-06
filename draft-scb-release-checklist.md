
# Table of Contents

1.  [Release Checklist](#orgbbda68d)
    1.  [Check third parties' licenses](#org24ee565)
    2.  [Check binary files](#org66afefc)
    3.  [License headers](#orgf198112)
    4.  [LICENSE](#org0180557)
    5.  [NOTICE](#org3ef2762)
    6.  [DISCLAIMER](#orgb1d94c5)
    7.  [SIGNING](#orgcc26a08)
2.  [References](#orgd628c91)
    1.  [Category A](#org0ca8296)
    2.  [Category B](#orge778c10)
    3.  [Category X](#orgc3e42a1)


<a id="orgbbda68d"></a>

# Release Checklist


<a id="org24ee565"></a>

## Check third parties' licenses

-   Third parties licensed under [Category A](#org0ca8296) can be used and distributed in source and binary form.
-   Third parties licenced under [Category B](#orge778c10) can only be used and distributed in binary form.
-   Third parties licensed under [Category X](#orgc3e42a1) can not be distrubed in either source or binary form. Can be used as tools in building and testing etc.

**Note**:
Take extra caution for javascript files. 

-   They may be minified thus lacking proper licensing information.
-   Different versions of the same library may have different licenses.
-   Libraries may bundle other third parties which use different licenses.


<a id="org66afefc"></a>

## Check binary files

-   images
    Distribution cannot included images that is properly licensed.
-   fonts
    Check the license of the font. The meta-data in the font file may not be accurate, check the original source.


<a id="orgf198112"></a>

## License headers

All source files must contain the ASL license header and does not contain a copyright line. This can be checked using rat.


<a id="org0180557"></a>

## LICENSE

Both the binary and source release **must** contain a LICENSE file containing all the licenses that the distribution used, including bundled third party components.

**Note**:
The binary and source release may have different LICENSE. The content of the LICENSE file **must** include the exactly necessary information.


<a id="org3ef2762"></a>

## NOTICE

Both the binary and source release **must** contain a NOTICE file containing the following contents:

-   The product copyright line
    Apache [PRODUCT<sub>NAME</sub>]
    Copyright [XXXX-XXXX] The Apache Software Foundation
    
    This product includes software developed at
    The Apache Software Foundation (<http://www.apache.org/>).
-   Anything legally required
-   Third party components' NOTICE
    Example: [hadoop's NOTICE](https://github.com/apache/hadoop/blob/trunk/NOTICE.txt)
-   Optional third party components     
    Example:
    This product optionally depends on 'JZlib', a re-implementation of zlib in
    pure Java, which can be obtained at:
    -   LICENSE:
        -   license/LICENSE.jzlib.txt (BSD style License)
    -   HOMEPAGE:
        -   <http://www.jcraft.com/jzlib/>

**Note**:
The binary and source release may have different NOTICE. The content of the NOTICE file **must** include the exactly necessary information.


<a id="orgb1d94c5"></a>

## DISCLAIMER

The following DISCLAIMER **must** be included for incubating projects:

Apache [Podling-Name] is an effort undergoing incubation at The Apache Software Foundation (ASF), sponsored by [the name of Apache TLP sponsor]. Incubation is required of all newly accepted projects until a further review indicates that the infrastructure, communications, and decision making process have stabilized in a manner consistent with other successful ASF projects. While incubation status is not necessarily a reflection of the completeness or stability of the code, it does indicate that the project has yet to be fully endorsed by the ASF.


<a id="orgcc26a08"></a>

## SIGNING

The final package must be cryptographically signed. It's better to use an apache.org email for signing.
PMC members voting +1 can also provide their signing signature.


<a id="orgd628c91"></a>

# References


<a id="org0ca8296"></a>

## Category A

-   Apache License 2.0
-   Apache Software License 1.1. Including variants:
    -   PHP License 3.01
    -   MX4J License
-   BSD (without advertising clause). Including variants:
    -   BSD 2-clause
    -   BSD 3-clause
    -   DOM4J License
    -   PostgreSQL License
    -   Eclipse Distribution License 1.0
-   MIT/X11
-   ISC
-   ICU
-   University of Illinois/NCSA
-   W3C Software License
-   W3C Community Contributor License Agreement - if at least 45 days after publication
-   X.Net
-   zlib/libpng
-   FSF autoconf license
-   DejaVu Fonts (Bitstream Vera/Arev licenses)
-   Academic Free License 3.0
-   Service+Component+Architecture+Specifications
-   OOXML XSD ECMA License
-   Microsoft Public License (MsPL)
-   Creative Commons Copyright-Only Dedication
-   Python Software Foundation License
-   Adobe Postcript(R) AFM files
-   Boost Software License Version 1.0
-   License for CERN packages in COLT but note that this applies only to CERN packages in COLT and not others
-   UK Open Government License. This license allows the licensor to provide a custom attribution notice. If one is provided, include in the NOTICE. If one is not provided, include 'Contains public sector information licensed under the Open Government Licence v3.0.' in the NOTICE.
-   WTF Public License
-   UNICODE, INC. LICENSE AGREEMENT - DATA FILES AND SOFTWARE
-   Zope Public License 2.0
-   ACE license
-   Oracle Universal Permissive License (UPL) Version 1.0


<a id="orge778c10"></a>

## Category B

-   Common Development and Distribution Licenses: CDDL 1.0 and CDDL 1.1
-   Common Public License: CPL 1.0
-   Eclipse Public License: EPL 1.0
-   IBM Public License: IPL 1.0
-   Mozilla Public Licenses: MPL 1.0, MPL 1.1, and MPL 2.0
-   Sun Public License: SPL 1.0
-   Open Software License 3.0
-   Erlang Public License
-   UnRAR License (only for unarchiving)
-   SIL Open Font License
-   Ubuntu Font License Version 1.0
-   IPA Font License Agreement v1.0
-   Creative Commons Attribution (CC-BY) 2.5, 3.0, and 4.0
-   Ruby License (including the older version when GPLv2 was a listed alternative Ruby 1.9.2 license)
-   Eclipse Public License 2.0: EPL 2.0


<a id="orgc3e42a1"></a>

## Category X

-   Binary Code License (BCL)
-   Special exceptions to the GNU GPL (e.g. GNU Classpath)
-   GNU GPL 1, 2, 3
-   GNU LGPL 2, 2.1, 3
-   GNU Affero GPL 3
-   NPL 1.0/NPL 1.1
-   QPL
-   Sleepycat License
-   Code Project Open License (CPOL)
-   BSD-4-Clause/BSD-4-Clause (University of California-Specific)
-   Field of use restrictions:
-   Microsoft Limited Public License
-   Amazon Software License (ASL)
-   JSON License
-   Non-commercial licenses:
-   Creative Commons Non-Commercial variants
-   Sun Community Source License 3.0
-   Facebook BSD+Patents license

