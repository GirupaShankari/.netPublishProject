pipeline {
   agent any

   stages {
   
      stage('Deploy') {
         steps {      
        //  bat  C:/"Program Files (x86)"/IIS/"Microsoft Web Deploy V3"/msdeploy.exe -verb:sync -source:package="Publish.zip" -dest:auto -setParam:name="IIS Web Application Name",value="Default Web Site/Publish"
        bat label: '', script: ' C:/"Program Files (x86)"/IIS/"Microsoft Web Deploy V3"/msdeploy.exe -verb:sync -source:package="Publish.zip" -dest:auto -setParam:name="IIS Web Application Name",value="Default Web Site/Publish"'
         }
      }

  /*    stage('Upload Zip To Nexus'){
            steps{
                script{

                   nexusArtifactUploader artifacts: [
                        [
                            artifactId: 'Publish.zip', 
                            classifier: '', 
                            file: "Publish.zip", 
                            type: 'zip'
                        ]
                    ], 
                    credentialsId: 'nexus3', 
                    groupId: 'in.javahome', 
                    nexusUrl: '10.61.43.73:8081', 
                    nexusVersion: 'nexus3', 
                    protocol: 'http', 
                    repository: 'simpleapp-release', 
                    version: "1" 
                   
                  /*  nexusArtifactUploader artifacts: [
                        [
                            artifactId: 'mySecondZipFile', 
                            classifier: '', 
                            file: "Installation of Nexus Repository on Windows.zip", 
                            type: 'zip'
                        ]
                    ], 
                    credentialsId: 'nexus3', 
                    groupId: 'in.javahome', 
                    nexusUrl: '10.79.244.15:8081', 
                    nexusVersion: 'nexus3', 
                    protocol: 'http', 
                    repository: 'simpleapp-release', 
                    version: "1" */
                    
                    
                    }
            }
        }*/
   }
}
