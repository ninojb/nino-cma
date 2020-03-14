# nino-cma
# Description
Car Maintenance App Repository. The aim of this repo is to have a logical place to store CMA related customisation.

# Instructions on adding this repo to the project

- **Clone this repo in the root directory of the project**

- **Add package directory to project**

Add the below script in  sfdx-project.json file under "packageDirectories". Ensure that the file is in valid JSON format, and "default" attribute is set to TRUE and other "default" attribute is set to FALSE. This will tell the CLI that you are working on this folder for the project.

```
{
  "path": "nino-base",
  "default": true
}
```

- **Add the below as part of .forceignore**

```
nino-cma/README.md
```

- **Push the codes**

```
sfdx force:source:push
```

- **Assign the permission Set to the user**

```
sfdx force:user:permset:assign -n Car_Maintenance_App_Access
```