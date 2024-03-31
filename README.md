refer this document to setup the ingress controler node " https://docs.aws.amazon.com/eks/latest/userguide/lbc-helm.html " <br />
launch the deployment-pods and services to connect with the ingress controller <br />
create ingressclass using the ALB/NLB/ELB/CLB <br />
use the ingressclass name to edit the annotation rules and setup the routes/path to  the services. using the ingress.yml <br />
**Note:** <br />
  - given paths should be created inside server/hosting file. like in server.js app.get("/home") <br />
         - now, the route  /home can be able to connect using the ingerss rules. <br />
to see the entire flow : aws -> EC2 -> ELB_services -> k8s-default-mynewing-3f7a199b19 -> click on( Resource map - new ) at bottom <br />
![Screenshot 2024-03-31 165042](https://github.com/naiduharinadh/k8s_ingress_worker/assets/137928332/c88e135e-aa55-4ea8-be70-426c46819aa2)
