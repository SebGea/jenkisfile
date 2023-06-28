pipeline {
agent any
parameters {
string(name: 'NAME', description: 'Nom ?')
string(name: 'NAME', description: 'Nom ?')
choice(name: 'GENDER', choices: ['Male', 'Female'], description: 'Sexe ?)
}
stages {
    stage('Printing name') {
        steps {
            script {
                def name = "${params.NAME}"
                def gender = "${params.GENDER}"
                if(gender == "Male") {
                echo "Mr. $name"
                        }
                else {
                echo "Mrs. $name"
                }
            }
        }
    }

    stage('BUILD') {
            steps {
                echo 'Developpement'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('DEPLOY') {
            steps {
                echo 'Mise en Production'
            }
        }
    }
}
