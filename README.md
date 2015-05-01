REF: http://www.journaldev.com/3531/spring-mvc-hibernate-mysql-integration-crud-example-tutorial

0) Create the project under git folder with maven tool;
*******************************************************
mvn archetype:generate -DgroupId=com.journaldev.spring -DartifactId=SpringMVCHibernate -DarchetypeArtifactId=maven-archetype-webapp -DinteractiveMode=false

1) Create a new project on github with name: 'SpringMVCHibernate'
*****************************************************************

2) Create the project under git folder with maven tool;
*******************************************************
echo # SpringMVCHibernate >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:bzdgn/SpringMVCHibernate.git
git push -u origin master

3) Import the project into eclipse workspace as "existing maven project"
************************************************************************

4) Update pom file and execute "mvn clean install"
**************************************************

5) Update web.xml file as per tutorial
**************************************

6) Update all sources as per tutorial
*************************************

7) Check deployment assembly on eclipse if Maven Dependencies are ok ( for Tomcat )
***********************************************************************************

8) Update context-param on web.xml, tutorial using the root-context which is neither needed nor working;
**********************************&&&*******************************************************************
Old value;
    <context-param>
        <param-name>contextConfigLocation</param-name>
        <param-value>/WEB-INF/spring/root-context.xml</param-value>
    </context-param>

New Value;
	<context-param>
		<param-name>contextConfigLocation</param-name>
		<param-value>/WEB-INF/spring/appServlet/servlet-context.xml</param-value>
	</context-param>
