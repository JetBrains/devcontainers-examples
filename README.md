# devcontainers-examples
Examples of using DevContainers with JetBrains IDE.

## DevContainers - reproducible development environments
The DevContainers approach allows for placing a fully functional development environment in containers:
- Running applications
- Running IDEs and tooling
- Appropriate versions of libraries and dependencies
- Runtimes required by a specific codebase and project, used in continuous integration and testing.
- Simple onboard new people (The development environment is configured automatically.)
- The goal of DevContainers is to provide a fully functional, reproducible development environment along with an IDE.

DevContainers help save a lot of time setting up the development environment, especially during the onboarding of new employees to a project.
For new colleagues, it often translates to reading tons of documentation.
Besides coding, developers frequently spend time figuring out which dependencies are needed to make the code work.
Or the code was written on macOS and for some reason, it doesn't work when run on Windows. What could have gone wrong? :)

JetBrains development environments are introducing built-in support for DevContainers.
DevContainers come pre-configured with the required environments and dependencies as needed for your project.
You can also create your own DevContainer and customize it once, then use it as much as needed.
In DevContainers, the source code of your application becomes available without the need for manual uploading
(via source mounting or creating a DevContainer from a repository over SSH).

When you connect to a DevContainer, your developer experience is the same as when working locally.
This works thanks to the Remote Development technology, where an IDE server runs inside the container and a local frontend,
which exchange only the changes in the view in a very fast and efficient manner thanks to the RD protocol.

In this repository, you will find several examples that will help you learn how to use DevContainers with the JetBrains 2023.3+ IDEs release.

**Examples**

`/.devcontainer/0-minimal_*` - base OS examples

`/.devcontainer/1-spec_*` - еxamples of using devcontainer.json options.

`/.devcontainer/1-features_*` - features examples

`/.devcontainer/2-compose_*` - compose examples

