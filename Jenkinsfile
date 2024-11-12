pipeline { 
     agent any 
     stages { 
          stage("Compile") { 
               steps { 
                    sh "chmod +x ./gradlew"
                    sh "./gradlew compileJava" 
               } 
          }
            stage("Build") {
                         steps {
                              sh "./gradlew build"
                         }
                    }

          stage("Unit test") { 
               steps { 
                    sh "./gradlew test" 
               } 
          } 
     } 
} 
