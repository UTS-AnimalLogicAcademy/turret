# turret

Turret is a tool which connects [Autodesk's Shotgun](https://www.shotgunsoftware.com/) and [Pixar's USD](https://graphics.pixar.com/usd/docs/index.html) to create a light-weight file resolver architecture that works across a range of content creation software. Turret is built around a workflow that allows assets to push updates down stream rather than the more manual and traditional alternative of artists needing to pull assets when needed. This works well in smaller development teams and for us at the [UTS Animal Logic Academy](https://animallogicacademy.uts.edu.au/). 

Turret has been developed by students and staff at the [UTS Animal Logic Academy](https://animallogicacademy.uts.edu.au/) over the last three years and is used throughout almost every stage of production.

This repository functions as a portal to each of the other corresponding turret repositories.

## Usage

There are two components to turret. [turret_server](https://github.com/UTS-AnimalLogicAcademy/turret_server) which runs in the background on artists workstations, and some extension of [turret_lib](https://github.com/UTS-AnimalLogicAcademy/turret_lib). Building instructions can be found inside each repository.

### Server

[turret_server](https://github.com/UTS-AnimalLogicAcademy/turret_server) requires pyzmq and [turret_server](https://github.com/UTS-AnimalLogicAcademy/turret_resolver).

 * [turret_resolver](https://github.com/UTS-AnimalLogicAcademy/turret_resolver)
 * [turret_server](https://github.com/UTS-AnimalLogicAcademy/turret_server)

### Client

[turret_lib](https://github.com/UTS-AnimalLogicAcademy/turret_server) is a DCC agnostic, C++ library that handles calls back to a [turret_server](https://github.com/UTS-AnimalLogicAcademy/turret_server). For us we mainly use [turret_usd](https://github.com/UTS-AnimalLogicAcademy/turret_usd) and [turret_klf](https://github.com/UTS-AnimalLogicAcademy/turret_klf) which both extend [turret_lib](https://github.com/UTS-AnimalLogicAcademy/turret_lib). More information can be found in their respective repositories.

 * [turret_lib](https://github.com/UTS-AnimalLogicAcademy/turret_lib)
 * [turret_usd](https://github.com/UTS-AnimalLogicAcademy/turret_usd)
 * [turret_klf](https://github.com/UTS-AnimalLogicAcademy/turret_klf)

## Awards

Turret won an award at [Shotgun's 5th annual pipeline awards](https://www.shotgunsoftware.com/blog/congrats-to-shotguns-4-new-pipeline-award-winners/) during SIGGRAPH 18. 
![Shotgun's 5th annual pipeline awards](https://www.shotgunsoftware.com/dynamic_resources/sg_blog_post_content/302/html_content/11539122970.png)

## Contributing
We use turret across almost every aspect of our USD pipeline and are constantly fixing bugs and finding time to improve turret more and more. We are however, very open to external pull-requests, and growing turret into a more versatile and robust piece of software with your help. Feel free to get in contact directly or through these GitHub repos. We'd love to talk! 
