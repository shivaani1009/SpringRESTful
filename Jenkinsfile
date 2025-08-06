pipeline{
agent any
tools {maven: "mavenv3"}
stages{
stage("Checkout"){
  steps{
    git branch: "main", url: "https://github.com/shivaani1009/SpringRESTful.git"
  }
}
stage("build"){
    steps{
      sh "mvn compile"
    }
}
stage("test"){
    steps{
      sh "mvn test"
    }
}
}
}
