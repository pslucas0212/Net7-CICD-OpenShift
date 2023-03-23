# .Net 7 development CI/CD Pipeline to OpenShift

For this tutorial you will need an OpenShift cluster to deploy your .Net application.  I will use the test OCP cluster that I created in a previous tutorial, [OpenShift 4.12 vSphere Installer Provisioned Infrastructure Tutorial](https://github.com/pslucas0212/OCP4.12-IPI-vSphere-Install), to demonstrate .Net 7 development on a Mac

This tutorial [Run .Net 7 code on Red Hat OpenShift Container Platform on MacOS](https://cloud.redhat.com/blog/run-.net-7-code-on-red-hat-openshift-container-platform-on-macos) how to setup a basic .Net 7 development environment on your Mac.

### Install the OpenShift Command Line Client
- Download the Mac OCP command line client

.... List steps here ...

- Untar openshift-client-mac.tar file in the Downloads directory
```
 % tar xvf Downloads/openshift-client-mac.tar 
x README.md
x oc
x kubectl
```
- Move the oc and kubectl files to the /usr/local/bin directory
```
% sudo mv oc kubectl /usr/local/bin
```

### Login in to your OCP cluster
- To run OCP CLI tool you will need to update your security settings on the Mac.  Run oc on the command line and the go to the Settings | Secuirty & Privacy dialog box.  On the General tab unlock the padlock to allow oc to run.  Click the Allow Anway button.
![Security & Privacy - Allow Anyway]()

- Run the oc command again and from the popup dialog box, click the Open button
![Open Button]()


- To login in to your OCP cluster the first time from your Mac, you will be prompted to provide other information.you will need the cluster API URL.
