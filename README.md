clb_mvnrepo
===========

Cloudburo public maven repository. The GIT repository consists of the two branches 'snapshots' and 'release' which will contain Cloudburo artifacts released for direct Maven integration. In order to connect to this repository from a Maven POM you have to add the following entries:

      <repositories>
    	<repository>  
        	<id>clb-mvnrepo-snapshots</id>  
        	<name>Cloudburo Maven Repo Snapshot on Github</name>  
        	<releases><enabled>false</enabled></releases>
            <snapshots><enabled>true</enabled></snapshots>
        	<url>https://raw.github.com/talfco/clb_mvnrepo/raw/snapshots</url>  
    	</repository>
    	 <repository>  
        	<id>clb-mvnrepo-release</id>  
        	<name>Cloudburo Release Repo on Github</name>  
        	<releases><enabled>true</enabled></releases>
            <snapshots><enabled>false</enabled></snapshots>
        	<url>https://raw.github.com/talfco/clb_mvnrepo/raw/release</url>  
    	</repository>
    </repositories>
