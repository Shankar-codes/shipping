@Library('jenkins-shared-library') _

def configMap = [
    project: "roboshop",
    component: "shipping"
]

echo "Going to execute Jenkins shared library"
// if branch is not equal to main, then run CI pipeline
if ( ! env.BRANCH_NAME.equalsIgnoreCase('main') ){
    javaEKSPipeline(configMap)
}
else {
    echo "Please follow the CR process"
}