## 引用/使用三方代码

1. 引用三方依赖，代码库中不包含被引用的代码。

  a. 以源代码发布时，不需要提及未包含的被引用三方依赖。

  b. 以二进制形式发布时，如果包含了被引用三方依赖，需要修正NOTICE文件，声明三方版本号，源地址以及所属许可协议。如果被包含的三方代码有NOTICE，必须将其NOTICE原样拷贝至项目NOTICE文件中。需要修正LICENSE文件，声明包含三方库版本和所属许可协议。
      
 *注意* 对于三方依赖的依赖，只要在发布时包含了其内容，和直接依赖没有区别，需要等同处理。

2. 直接将三方代码拷贝进项目（单个文件，文件夹，或者代码片断）。
  
  不要对被拷贝代码的许可协议和版权声明做任何修改。
  
  对于拷贝的代码片断，需要在拷贝处注明来源，许可协议和版权声明。
  
  必须在项目的LICENSE文件中，声明拷贝代码的地址，源地址和许可协议。
  
  必须在项目的NOTICE文件中添加拷贝代码的版权声明。
  
  如果被拷贝的三方代码有NOTICE，必须将其NOTICE原样拷贝至项目NOTICE文件中。

  *注意* 拷贝源代码的版权声明至NOTICE文件中时，对于Apache 2.0许可的代码，需要将免责声明一起拷贝。对于其它许可的通常拷贝版权声明和所属许可即可。操作时请注意分析。

3. 贡献者提交的非Apache 2.0 License的代码。
  
  必须在项目LICENSE文件中声明贡献代码的路径和所属许可协议。


## 示例

### LICENSE

```
                                 Apache License
                           Version 2.0, January 2004
                        http://www.apache.org/licenses/

   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION

=== 第一部分，Apache License 2.0 ===
   

=======================================================================
Apache Spark Subcomponents:

The Apache Spark project contains subcomponents with separate copyright
notices and license terms. Your use of the source code for the these
subcomponents is subject to the terms and conditions of the following
licenses.


========================================================================
For heapq (pyspark/heapq3.py):
========================================================================

See license/LICENSE-heapq.txt

=== 第二部分，拷贝的三方代码，贡献者提交的非Apache 2.0代码 ===

========================================================================
BSD-style licenses
========================================================================

The following components are provided under a BSD-style license. See project link for details.
The text of each license is also included at licenses/LICENSE-[project].txt.

     (BSD 3 Clause) netlib core (com.github.fommil.netlib:core:1.1.2 - https://github.com/fommil/netlib-java/core)
     (BSD 3 Clause) JPMML-Model (org.jpmml:pmml-model:1.2.7 - https://github.com/jpmml/jpmml-model)
     (BSD License) AntLR Parser Generator (antlr:antlr:2.7.7 - http://www.antlr.org/)
     (BSD License) ANTLR 4.5.2-1 (org.antlr:antlr4:4.5.2-1 - http://wwww.antlr.org/)
     (BSD licence) ANTLR ST4 4.0.4 (org.antlr:ST4:4.0.4 - http://www.stringtemplate.org)

=== 第三部分，打包发布的三方依赖 ===     
```

### NOTICE
```
Apache Spark
Copyright 2014 and onwards The Apache Software Foundation.

This product includes software developed at
The Apache Software Foundation (http://www.apache.org/).

=== 第一部分，项目本身的声明 ===

========================================================================
Common Development and Distribution License 1.0
========================================================================

The following components are provided under the Common Development and Distribution License 1.0. See project link for details.

     (CDDL 1.0) Glassfish Jasper (org.mortbay.jetty:jsp-2.1:6.1.14 - http://jetty.mortbay.org/project/modules/jsp-2.1)
     (CDDL 1.0) JAX-RS (https://jax-rs-spec.java.net/)
     (CDDL 1.0) Servlet Specification 2.5 API (org.mortbay.jetty:servlet-api-2.5:6.1.14 - http://jetty.mortbay.org/project/modules/servlet-api-2.5)
     (CDDL 1.0) (GPL2 w/ CPE) javax.annotation API (https://glassfish.java.net/nonav/public/CDDL+GPL.html)
     (COMMON DEVELOPMENT AND DISTRIBUTION LICENSE (CDDL) Version 1.0) (GNU General Public Library) Streaming API for XML (javax.xml.stream:stax-api:1.0-2 - no url defined)
     (Common Development and Distribution License (CDDL) v1.0) JavaBeans Activation Framework (JAF) (javax.activation:activation:1.1 - http://java.sun.com/products/javabeans/jaf/index.jsp)

=== 第二部分，包含的三方依赖版权列表 ===

========================================================================
NOTICE files
========================================================================

The following NOTICEs are pertain to software distributed with this project.


// ------------------------------------------------------------------
// NOTICE file corresponding to the section 4d of The Apache License,
// Version 2.0, in this case for
// ------------------------------------------------------------------

Apache Avro
Copyright 2009-2013 The Apache Software Foundation

This product includes software developed at
The Apache Software Foundation (http://www.apache.org/).

=== 第三部分，包含的三方依赖的NOTICE ===

===============================================================================
For dev/sparktestsupport/toposort.py:

Copyright 2014 True Blade Systems, Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

=== 第四部分，拷贝的三方代码版权声明 ===
```
