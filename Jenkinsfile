piprline {
    agent any
    stages {
        stage ('one') {
            steps {
                echo 'Hi! this is harikrishna'
            }
        }
      satage('two') {
        steps {
            input ('Do you want to proceed?')
        }
    }
  stage ('three') {
    when {
        not {
            branch "master"
        }
    }
    steps {
        echo "Hello"
    }
}
stage ('four')
parallel {
    satge ("unit test") {
        steps {
            echo "running the unit testing"
        }
    }
    satge ('integration test') {
    agent {
        docker {
            resuse node false 
            "image ubuntu"
            
        }
    }
    steps { 
        echo "running the integraration test--"
    }
 }
}
}
}
}


