# Jenkins For Android CI

See docker-compose.yml for how to use this.

To start the containers
		docker-compose up

The Jenkins home directory is stored in a separate data container, along with the extra Android SDK components.

This image only comes with the base Android SDK, you'll need to install the components you want to use.
		docker exec -it android-template bash

Then the usual `android update-sdk` command with the appropriate options.

If you want to just build the image:
		docker build -t android-jenkins .
