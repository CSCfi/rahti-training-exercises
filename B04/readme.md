# Create Service and Route

> Pre-requisites, the Pod created in *[Exercise 3](/exercises/B03/index.html)*

In this exercise we will make the pod accessible to the whole Internet, using a HTTPS URL.

## Create a Service

* From the 'Application console', create a service called [hello-service](/exercises/B04/hello-service.yaml) that load balances the Pod from exercise 2.

* From the 'Application console':
    * Check that the selector is `app=hello-pod`
    * Check the IP of the service (it should begin by `172`)
    * Check the list of Pods, you should see the Pod created in Exercise 2.

**Advanced**: Try to understand what is what links this Service with this Pod.

## Create a Route

* From the Application console, create a Route using the form. User the Service create in the previous step (Should be only available anyway), make the route secure (HTTPS), and let Rahti choose the Host-name URL.
    * Check which host-name URL was auto generated and using the browser, go to that URL.
    * Go back to the Pod's log and see if your visit has been logged.
