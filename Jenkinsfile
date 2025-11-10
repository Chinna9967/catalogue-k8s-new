// #!groovy
// @Library('roboshop-shared-library') _

// def configMap = [
//     application: "nodeJSEKS",  // we are migrating monolithic(VM) to microservices(container,pod)
//     component: "catalogue"
// ]
// env
// // this is .groovy file name and function inside it
// // if not master branch then trigger pipeline
// if ( ! env.BRANCH_NAME.equalsIgnoreCase("master")) {
//     pipelineDecission.decidePipeline(configMap)
// }
// else{
//     echo "master deployment should happen through cr only"
// }

// // pipelineDecission.decidePipeline(configMap)

@Library('roboshop-shared-library') _

def configMap = [
    application: "nodeJSEKS",
    component: "catalogue"
]

if (!env.BRANCH_NAME.equalsIgnoreCase("master")) {
    pipelineDecission.decidePipeline(configMap)
} else {
    echo "master deployment should happen through cr only"
}
