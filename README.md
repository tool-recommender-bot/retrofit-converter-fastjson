FastJson Retrofit Converter
===================
[![Build Status](https://travis-ci.org/ligboy/retrofit-converter-fastjson.svg?branch=master)](https://travis-ci.org/ligboy/retrofit-converter-fastjson)
converter-fastjson[![Download](https://api.bintray.com/packages/ligboy/maven/retrofit-converter-fastjson/images/download.svg)](https://bintray.com/ligboy/maven/retrofit-converter-fastjson/_latestVersion)
converter-fastjson-android[![Download](https://api.bintray.com/packages/ligboy/maven/retrofit-converter-fastjson-android/images/download.svg)](https://bintray.com/ligboy/maven/retrofit-converter-fastjson-android/_latestVersion)

Retrofit ships with support for OkHttp's `RequestBody` and `ResponseBody` types but the library is
content-format agnostic. This modules contained herein are additional converters for JSON which uses FastJson.
For more information please see [the website][1].

Download
--------

Download the latest JAR: [converter-fastjson][2] [converter-fastjson-android][3].  
### Via Maven:
#### dependency:
```xml
<dependency>
  <groupId>org.ligboy.retrofit2</groupId>
  <artifactId>converter-fastjson</artifactId>
  <version>2.1.0</version>
</dependency>
```
 *For fastjson-android:*
```xml
<dependency>
  <groupId>org.ligboy.retrofit2</groupId>
  <artifactId>converter-fastjson-android</artifactId>
  <version>2.1.0</version>
</dependency>
```
### or Gradle:
#### dependency:
```groovy
compile 'org.ligboy.retrofit2:converter-fastjson:2.1.0'
```
 *For fastjson-android:*
```groovy
compile 'org.ligboy.retrofit2:converter-fastjson-android:2.1.0'
```
Usage
-------
FastJson Retrofit Converter requires at minimum Java 7 or Android 2.3.
To use, supply an instance of your desired converter when building your `Retrofit` instance.

```java
Retrofit retrofit = new Retrofit.Builder()
  .baseUrl("https://api.example.com")
  .addConverterFactory(FastJsonConverterFactory.create())
  .build();
```

#### Deploy
```bash
mvn deploy --settings settings
```
License
=======
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

 [1]: http://square.github.io/retrofit/
 [2]: https://bintray.com/ligboy/maven/retrofit-converter-fastjson/_latestVersion
 [3]: https://bintray.com/ligboy/maven/retrofit-converter-fastjson-android/_latestVersion
