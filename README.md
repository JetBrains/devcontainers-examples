# devcontainers-examples
Examples of using DevContainers with JetBrains IDE (WIP).

## DevContainers - reproducible development environments
The DevContainers approach allows for placing a fully functional development environment in containers:
- Running applications
- Running IDEs and tooling
- Appropriate versions of libraries and dependencies
- Runtimes required by a specific codebase and project, used in continuous integration and testing.
- Simple onboard new people (The development environment is configured automatically.)
- Utilize remote development capabilities, working with code on a server equipped with Docker and necessary hardware

The goal of DevContainers is to provide a fully functional, reproducible development environment along with an IDE.

DevContainers help save a lot of time setting up the development environment, especially during the onboarding of new employees to a project.
For new colleagues, it often translates to reading tons of documentation.
Besides coding, developers frequently spend time figuring out which dependencies are needed to make the code work.

JetBrains development environments are introducing built-in support for DevContainers.
DevContainers come pre-configured with the required environments and dependencies as needed for your project.
You can also create your own DevContainer and customize it once, then use it as much as needed.
In DevContainers, the source code of your application becomes available without the need for manual uploading
(via source mounting or creating a DevContainer from a repository over SSH).

When you connect to a DevContainer, your developer experience is the same as when working locally.
This works thanks to the Remote Development technology, where an IDE server runs inside the container and a local frontend,
which exchange only the changes in the view in a very fast and efficient manner thanks to the RD protocol.

## How to create a Dev Container
The *devcontainer.json* file in your project instructs IDE how to create a development
container with a predefined tool and runtime stack.

The devcontainer.json file can be located in one of the following paths in the project:</p>
 - .devcontainer/devcontainer.json
 - .devcontainer.json
 - .devcontainer/<folder>/devcontainer.json (where <folder> is a sub-folder, one level deep)

## How to build and run a Dev Container
[Please read in the official documentation](https://www.jetbrains.com/help/idea/connect-to-devcontainer.html#start_from_gateway)

### Dependencies
Requires *Docker* installed on a local machine.

Remote Development may require some dependencies in the Dev Container, such as *curl*, *unzip*, *ps*, *libxext*, *libxrender*, 
*libxtst*, *libxi*, *freetype*, *procps*, *gcompat*.

If your dev container doesn't start, try installing them (see more in the 0*-minimal examples). 

We are working to reduce the number of Remote Development dependencies in future releases.

[JetBrains IDE Plugin](https://plugins.jetbrains.com/plugin/21962-dev-containers)

## Examples

`/.devcontainer/0*-minimal_*` - base OS examples

`/.devcontainer/1*-spec_*` - еxamples of using devcontainer.json options.



