

TODO
----
* [IN PRG] Update README
* Use namespace, remove class prefixes, move header files to subdirectory,
   provide automated refactoring tips and insttructions to users. 
* Change installation locations to match current OS standards (Linux and
  Windows)
* Change robot parameter file loading to check user home directory 
* Remove ArStringInfoGroup (merge with data logger, let classes
  supply data accessors for data logger or other higher level uses 
  such as UI, middleware, etc.)
* Remove barriers to simpler wrapper libraries (swig and non-swig)
* Separate into multiple libraries (with optional full aria build also for
  compatibilty)?  -- aria-core, aria-devices, aria-actionlib? 
* Continue to reduce number of classes needed for typical applications.
  Reduce boilerplate needed on new programs. simpleConnect example should be <10
  lines of code.
* Reduce header dependencies. Fewer files should include Aria.h.  Eventually
  deprecate Aria.h?
* Remove ArDrawingData (move to ArNetworking registry of what sensor
  visualizations should look like, maybe configurable in server config file)
* [IN PRG] Remove various features in ARIA that are needed for ArNetworking/ARAM only.
* overhaul other documentation.  
* Add more data logger features.
* Consolidate src/*.cpp and include/*.h in aria/ subdirectories, should
  match header installation directory.  
* Move matlab/ariac to ariac/. Update matlab and rust builds.
* Remove weird stuff in ArSystemStatus
* Set up Travis CI to test build (later tests).
* Switch to CMake?
* Start adding some real unit testing?
 

Maybe TODO eventually
----------

* Simplify ArMap.  (Restore from older version of ARIA without "Components"?)
* Possibly refactor ArRobot to be a smaller class. Separate robot communications
  and control/data API from other higher level features
* Replace old ArModuleLoader with similar
* Remove ArActions or move to another library.
* Move device interfaces to separate libraries?
* Add proper unit tests.
* Incorporate some ArNetworking replacement.  Generic mechanism for ARIA classes
  to expose methods (actions/callbacks) to UI or middleware layers.  (With multiple
  implementations possible in other libraries or code units, e.g. user custom, ROS, HTTP REST, etc.)
* Develop logging (ArLog) further.
* enums in config items
* replace ArFunctor with modern C++ replacement
* generally update to modern C++

