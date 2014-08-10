mvnrepository
=============

Maven Repository for ActionScript Development

URL
---

> https://raw.githubusercontent.com/vpmedia/mvnrepository/master

Content
-------

* Adobe AIR SDK 14.0
* Apache Flex SDK 4.13
* Apache FlexUnit 4.2
* Apache FlexPMD 1.3

License
-------

Mixed license binaries.

**

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.


Ivy Example
-----------

ivysettings.xml

    <ivysettings>
      <settings defaultResolver="chained"/>
      <resolvers>
        <chain name="chained">
          <ibiblio name="central.maven" root="http://central.maven.org/maven2/" m2compatible="true"/>
          <ibiblio name="vpmedia" root="https://raw.githubusercontent.com/vpmedia/mvnrepository/master" m2compatible="true"/>
          <ibiblio name="oss.sonatype" root="https://oss.sonatype.org/content/groups/public/" m2compatible="true"/>
          <ibiblio name="ibiblio" root="http://mirrors.ibiblio.org/pub/mirrors/maven2" m2compatible="true"/>
          <ibiblio name="java.net2" root="http://download.java.net/maven/2/" m2compatible="true"/>
        </chain>
      </resolvers>
    </ivysettings>

ivy.xml

    <dependencies>
        <dependency org="org.apache" name="flexunit-tasks" rev="4.2.0-20140410"/>
        <dependency org="org.apache" name="flexunit-as3" rev="4.2.0-20140410"><artifact name="flexunit-as3" type="swc"/></dependency>
        <dependency org="org.apache" name="flexunit-cilistener" rev="4.2.0-20140410"><artifact name="flexunit-cilistener" type="swc"/></dependency>
        <dependency org="org.apache" name="flexunit-uilistener" rev="4.2.0-20140410"><artifact name="flexunit-uilistener" type="swc"/></dependency>
        <dependency org="org.apache" name="hamcrest-as3" rev="1.1.3"><artifact name="hamcrest-as3" type="swc"/></dependency>
        <dependency org="org.apache" name="flex-pmd-ant-task" rev="1.3"/>
        <dependency org="org.apache" name="flex-pmd-files" rev="1.3"/>
        <dependency org="org.apache" name="flex-pmd-core" rev="1.3"/>
        <dependency org="org.apache" name="flex-pmd-ruleset" rev="1.3"/>
        <dependency org="org.apache" name="flex-pmd-ruleset-api" rev="1.3"/>
        <dependency org="org.apache" name="flex-pmd-cpd" rev="1.3"/>
        <dependency org="org.apache" name="flex-pmd-cpd-ant-task" rev="1.3"/>
        <dependency org="org.apache" name="flex-pmd-metrics" rev="1.3"/>
        <dependency org="org.apache" name="flex-pmd-metrics-ant-task" rev="1.3"/>
        <dependency org="org.apache" name="as3-parser" rev="1.3"/>
        <dependency org="org.apache" name="as3-parser-api" rev="1.3"/>
        <dependency org="org.apache" name="as3-plugin-utils" rev="1.3"/>
        <dependency org="pmd" name="pmd" rev="4.2.5"/>
        <dependency org="commons-lang" name="commons-lang" rev="2.4"/>
        <dependency org="org.codehaus.plexus" name="plexus-utils" rev="3.0.17"/>
    </dependencies>

Gradle Example
---------------

    repositories {
        mavenLocal()
        mavenCentral()
        maven {
            url 'https://raw.githubusercontent.com/vpmedia/mvnrepository/master'
        }
        maven {
            url 'https://oss.sonatype.org/content/groups/public/'
        }
    }

    dependencies {
        test group: 'org.apache', name: 'flexunit-tasks', version: '4.2.0-20140410', ext: 'jar'
        test group: 'org.apache', name: 'flexunit-as3', version: '4.2.0-20140410', ext: 'swc'
        test group: 'org.apache', name: 'flexunit-cilistener', version: '4.2.0-20140410', ext: 'swc'
        test group: 'org.apache', name: 'flexunit-uilistener', version: '4.2.0-20140410', ext: 'swc'
        test group: 'org.apache', name: 'hamcrest-as3', version: '1.1.3', ext: 'swc'
        test group: 'org.apache', name: 'flex-pmd-ant-task', version: '1.3', ext: 'jar'
        test group: 'org.apache', name: 'flex-pmd-files', version: '1.3', ext: 'jar'
        test group: 'org.apache', name: 'flex-pmd-core', version: '1.3', ext: 'jar'
        test group: 'org.apache', name: 'flex-pmd-ruleset', version: '1.3', ext: 'jar'
        test group: 'org.apache', name: 'flex-pmd-ruleset-api', version: '1.3', ext: 'jar'
        test group: 'org.apache', name: 'flex-pmd-cpd', version: '1.3', ext: 'jar'
        test group: 'org.apache', name: 'flex-pmd-cpd-ant-task', version: '1.3', ext: 'jar'
        test group: 'org.apache', name: 'flex-pmd-metrics', version: '1.3', ext: 'jar'
        test group: 'org.apache', name: 'flex-pmd-metrics-ant-task', version: '1.3', ext: 'jar'
        test group: 'org.apache', name: 'as3-parser', version: '1.3', ext: 'jar'
        test group: 'org.apache', name: 'as3-parser-api', version: '1.3', ext: 'jar'
        test group: 'org.apache', name: 'as3-plugin-utils', version: '1.3', ext: 'jar'
        test group: 'pmd', name: 'pmd', version: '4.2.5', ext: 'jar'
        test group: 'commons-lang', name: 'commons-lang', version: '2.4', ext: 'jar'
        test group: 'org.codehaus.plexus', name: 'plexus-utils', version: '3.0.17', ext: 'jar'
    }
