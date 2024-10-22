### K8s Crashloopbackoff 

* A CrashLoopBackOff is a common error in Kubernetes that indicates a container within a Pod is repeatedly crashing and restarting. This state arises when the container fails to start properly, leading Kubernetes to implement an exponential back-off strategy, where it increases the wait time between restart attempts. This delay starts at 10 seconds and can extend up to five minutes if the container continues to fail.

#### Init containers  

* Init containers in Kubernetes are specialized containers that run before the main application containers within a Pod. Their primary purpose is to perform initialization tasks, ensuring that any necessary setup or configuration is completed before the application begins executing. 
* Its like depends on statement.

* After writing a yaml file for running any application in K8s, 
     * Exposing Pod directly to external world is not a recommended practice, we are using the following only for evaluation.

##### Resources in Pods
* Resources refer to the computing power and memory that containers require to function effectively within a cluster
* It limits the memory which requires to run in  the pods
    * CPU 
    * RAM  
* It is of are two types 
  * requests # lower limits
  * limits # Upper limits 