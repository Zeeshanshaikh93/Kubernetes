### K8s Crashloopbackoff 

* A CrashLoopBackOff is a common error in Kubernetes that indicates a container within a Pod is repeatedly crashing and restarting. This state arises when the container fails to start properly, leading Kubernetes to implement an exponential back-off strategy, where it increases the wait time between restart attempts. This delay starts at 10 seconds and can extend up to five minutes if the container continues to fail.

#### Init containers  

* Init containers in Kubernetes are specialized containers that run before the main application containers within a Pod. Their primary purpose is to perform initialization tasks, ensuring that any necessary setup or configuration is completed before the application begins executing. 
* Its like depends on statement.