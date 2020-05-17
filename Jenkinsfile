pipelineJob("Test_1") {
   agent any

   stages {
      stage('Hello') {
         steps {
            echo 'Hello'
         }
      }
      stage('World') {
         steps {
            echo 'World'
         }
      }
      stage('Gradle Tasks') {
         steps {
            gradle {
               useWrapper(true)
               makeExecutable(true)
               tasks('whatIsMyName')
               switches('--debug')
            }
         }
      }
   }
}
