# Backstage vs. DHP Portal

## DHP Initializer

DHP Initializer allows users to create a start-up source code from a defined template. It can also:

- publish source code to Azure Gits.
- create an Azure pipelines.
- create a ticket for creating a SQLServers DB.
- ...

Software Template in Backstage is providing the similar functionality.

### Create a new initializer in Backstage and DHP Portal  

| Steps | Backstage | DHP Portal |
| ----| ---- | ---- |
| Initializers are developed and maintained by  | Any teams | DHP team |
| Create UI for collecting user input | Declared UI in the template file (done by Template author). <br /> Custom user input UI could be added as mentioned in [Writing Custom Field Extensions](https://backstage.io/docs/features/software-templates/writing-custom-field-extensions)  | Add new code for it (done by DHP Team) |
| Create skeleton files for generating source code | Skeleton files are template files of Template Engine [nunjucks](https://mozilla.github.io/nunjucks/) (done by Template author). <br /> Custom user input UI could be added as mentioned in [Writing Custom Field Extensions](https://backstage.io/docs/features/software-templates/writing-custom-field-extensions)  | No template engine is used (done by DHP Team) |
| Create actions of the initializer | Declared actions in the template file (done by Template author). <br /> Custom actions could be added as mentioned in [Writing Custom Actions](https://backstage.io/docs/features/software-templates/writing-custom-actions) | Create new code for actions (done by DHP Team) |

## DHP Documentation

Backstage Techdocs is a way to create document in Backstage. Initializer authors can create documents in [markdown](https://www.markdownguide.org/basic-syntax/) format. They will be built to html files.  
Along with Backstage's Software Catalog, the software template (initializer in DHP) and its document could be placed together.