pipeline {
  agent any
  stages {
    stage('stage_1') {
      steps {
        echo 'hello'
      }
    }

    stage('stage_2') {
      steps {
        sh '''mkdir -p build
echo "This is build number ${BUILD_NUMBER}" > build/release.txt
zip -r build.zip build'''
      }
    }

  }
}