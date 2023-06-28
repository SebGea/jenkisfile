pipeline {
       agent any
       parameters {
       string(name: 'NAME', description: 'Nom ?')
       string(name: 'FIRSTNAME', description: 'Prénom ?')
       choice(name: 'GENDER', choices: ['Homme', 'Femme'], description: 'Sexe ?')
       string(name: 'DATE', description: 'Date de naissance ?')
       string(name: 'AGE', description: 'Age ?')
       }
stages {
    stage('Parametres') {
        steps {
               script {
                     def prenom = "${params.FIRSTNAME}"
                     def nom = "${params.NAME}"
                     def genre = "${params.GENDER}"
                     def date = "${params.DATE}"
                     def age = "${params.AGE}"

                          echo "Bonjour $prenom $nom"
                          echo "Vous etes un(e) $genre."
                          echo "Vous etes né(e) le $date, vous avez $age ans."
                             sleep 5
                      }
              }
    }

        stage('Collection de datas') {
            steps {
                echo "Prise en compte de l'équipement..."
                sleep 5
                echo "Analyse en cours de la fréquence cardiaque..."
                sleep 5
                echo "Analyse en cours des différentes phases de sommeil..."
                sleep 5
                echo "Les analyses ont été réalisées avec succes."
            }
        }

        stage('Generation du Diagramme') {
            steps {
                echo "Génération du diagramme..."
                sleep 5 
                echo "Diagramme complété."
            }
        }   
}
}
