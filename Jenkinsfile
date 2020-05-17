pipeline {
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
            shell('echo START')
            gradle {
               useWrapper(true)
               makeExecutable(true)
               tasks('clean')
            }
         }
      }
   }
}
