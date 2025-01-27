# Dockerfile Test Execution Bug
This repository demonstrates a common error in Dockerfiles related to executing tests.  The original `Dockerfile` attempts to run unit tests using `unittest discover`, but fails because no test discovery mechanism is implemented. The `Dockerfile_fixed` provides a solution. 

**Bug:** The original `Dockerfile`'s `CMD` instruction tries to run tests using `unittest discover` without specifying where to discover them from. This results in a failure.

**Solution:** The `Dockerfile_fixed` includes changes to handle test discovery properly. 