

# TODO: repo name

## What is this?
This is...
<br />

## Motivation?
The goal is provide the user with an abstraction layer that only requires a few input variables from the user (5 at the moment). 
The user should be able to create the following, 
* A Google Project within the correct department and its folder structure, where the user can 
  * Enable if the project should be using a vpc-connector or not (default is false).
  * The project should also have "default services enabled" as well as an artifactory registry repository and a default building bucket available.
* One or more Google Cloud Run instance(s) (gcr) where each instance can be configured with, 
  * Arguments to the entrypoint of the gcr instance 
  * Environment variables passed to the gcr instance
  * Secrets (possibly from from secretmanager) passed as environment variables to the gcr instance
  * Annotations passed to the gcr instance, both for controlling egress and ingress. 
  * If it should attach to the vpc-connector (default is to attach if vpc connector is enabled for the project, but can be overridden per instance)

This should be possible for the user without writing/copy/pasting a single line of terraform code (**almost**). 
<br />
<br />
## Prerequisites 
To use anything in this guide you need to...
<br />
<br />

## How to use

1.
2.
3.
<br />

# FAQ ?

### How is this project structured ? 
The basic folder structure... 
```
top_folder/
 └── folder1
     ├── folder2
     │   └── fileX.file
     ├── folder3
     │   └── fileX.file
     └── folder5
         ├── folder6
         │   ├── fileX.file
         │   └── fileX.file
         ├── folder6
         │   ├── fileX.file
```
<br />

## How do I ... ?
Simply edit "modules/app/main.tf", 

```
code example
```

***Notes*** 

*Do I have any notes*
