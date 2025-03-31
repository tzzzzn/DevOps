1. What is K8S?
2. Why do we need this? Do we have other alternatives?
3. What is the Architecture?
4. What is EKS?
5. What can K8S do? What are its limitations?
   - K8S can take care of pods if they fail will recreate them.
   - If kubelet on worker node stops communicating with Master node then it will be marked as notReady. 
   - And these pods will be assigned to existing nodes if there is availability.
 - Limitations:
   - It can't create a new node if it needs to scaled.
   - It can't heal even the existing node.
 * To fix the limitation we use external tools if we are on cloud we use Auto Scaling groups and Cluster Auto Scaler or EKS.
6. 