node {

        stage('Checkout') {

            git url: 'https://github.com/jayashreebhukele/projectformaven.git',  branch: 'master'

            echo '****************CHECKOUT SUCCESSFUL****************'

        }

   stage('Build') {

		def mvn_version = 'maven_home'

		withEnv( ["PATH+MAVEN=${tool mvn_version}/bin"]) {

			sh 'mvn site'

			}

		}

}
