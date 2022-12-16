pipeline {

agent any

stages {

     stage(‘Checkout’) {

     steps {
           {
            git branch: 'terraform', credentialsId: 'me', url: 'https://github.com/ttnwt/TESTTERRA.git'
            }
     stage('TF Init$Plan')
                   
     }
  
     }

    stage (“terraform init”) {

    steps {

          sh (‘terraform init’)

           }

      }

      stage (“terraform Action”) {

        steps {

         echo “Terraform action is –> ${action}”

         sh (‘terraform ${action} –auto-approve’)

}

}

}

}

 
    //  stage('Continuous delivery')
    //                {
    //                 input message: 'Waiting for approval from executor', submitter: 'ttwnt'
    //                 deploy adapters: [tomcat8(credentialsId: 'prodep', path: '', url: 'http://172.31.95.153:8080')], contextPath: 'catenv', war: '**/*.war'
    //                }
    //  stage('TF Apply')
    //                {
    //                 sh 'terraform apply imput=false'
// }
}
