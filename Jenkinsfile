pipeline {
agent any
parameters {
string(name: 'NAME', description: 'Nom ?')
string(name: 'FIRSTNAME', description: 'Prénom ?')
choice(name: 'GENDER', choices: ['Homme', 'Femme'], description: 'Sexe ?)
string(name: 'DATE', description: 'Date de naissance ?')
string(name: 'AGE', description: 'Age ?')
       }}
stages {
    stage('Printing Parameters') {
        steps {
            echo "Bonjour ${params.FIRSTNAME} ${params.NAME}"
            echo "Vous etes un(e) ${params.GENDER}
            echo "Vous êtes né(e) le ${params.DATE}, vous avez ${params.AGE} ans.
        }
    }

        stage('Collection de datas') {
            steps {
                echo "Analyse en cours de la fréquence cardiaque..."
                sleep 5
                echo "Analyse en cours des différentes phases de sommeil..."
                sleep 5
                echo "Les analyses ont été réalisées avec succes."
            }
        }

        stage('Génération du Diagramme') {
            steps {
                echo "Génération du diagramme..."
                sleep 5 
                echo "Diagramme complété."
            }
        }   
}
