# lpsolve-java

[DockerHub](https://hub.docker.com/r/everpeace/lpsolve-java/)

A base docker image for running lpsolve(mixed-integer programming solver) from its java binding.

This docker image already installed JNI libraries and configured linking libraries (via `LD_LIBRARY_PATH`).

So, all you can do is executing `java` in the container.

Happy solving linear programming!!

Based on:

* [openjdk:java8-slim](https://hub.docker.com/_/openjdk/)
* [lpsolve 5.5.0.15](https://sourceforge.net/projects/lpsolve/)
* [java binding of lpsolve 5.5](http://lpsolve.sourceforge.net/5.5/Java/README.html)
  * JNI library is installed at `/usr/lib/lp_solve/liblpsolve55j.so`
  * `LD_LIBRARY_PATH` is already set to `/usr/lib/lp_solve`
  * jar file is installed at `/opt/lp_solve_5.5_java/lib/lpsolve55j.jar`
    * You can also use maveninzed version ([datumbox/lpsolve](https://github.com/datumbox/lpsolve))
