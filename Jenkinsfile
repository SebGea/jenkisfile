pipeline {
agent any
parameters {
string(name: 'NAME', description: 'Nom ?')
string(name: 'FIRSTNAME', description: 'Prénom ?')
choice(name: 'GENDER', choices: ['Homme', 'Femme'], description: 'Sexe ?)
string(name: 'DATE', description: 'Date de naissance ?')
string(name: 'AGE', description: 'Age ?')
}
stages {
    stage('Printing Parameters') {
        steps {
            echo "Bonjour ${params.FIRSTNAME} ${params.NAME}"
            echo "Vous etes un(e) ${params.GENDER}
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
