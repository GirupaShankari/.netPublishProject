pipeline {
   agent any

   stages {
   
      stage('Deploy') {
         steps {      
        //  bat  C:/"Program Files (x86)"/IIS/"Microsoft Web Deploy V3"/msdeploy.exe -verb:sync -source:package="Publish.zip" -dest:auto -setParam:name="IIS Web Application Name",value="Default Web Site/Publish"
      //  bat label: '', script: ' C:/"Program Files (x86)"/IIS/"Microsoft Web Deploy V3"/msdeploy.exe -verb:sync -source:package="Publish.zip" -dest:auto -setParam:name="Publish",value="Default Web Site/Publish"'
          bat label: '', script: ' C:/"Program Files (x86)"/IIS/"Microsoft Web Deploy V3"/msdeploy.exe -verb:sync -source:package="Publish.zip" -dest:auto,computerName="http://172.31.81.195/msdeploy.axd?site=my_iis_site",username=Techie_Girupa,password=Girupa28,authType=basic -allowUntrusted=true'
        
         }
      }

   }
}
