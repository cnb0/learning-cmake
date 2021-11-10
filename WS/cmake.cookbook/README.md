- 00. Setting Up Your System

            Obtaining the code
            Docker image
            Installing prerequisite software
            Getting CMake
            Compilers
            Build-automation tools
            Python
            Additional software
            BLAS and LAPACK
            Message passing interface (MPI)
            The Eigen linear algebra template library
            The Boost libraries
            Cross-compilers
            ZeroMQ, pkg-config, UUID, and Doxygen
            Conda build and deployment tools
            Testing the recipes
            Reporting problems and suggesting improvements

- 01. From A Simple Executable To Libraries

            Compiling a single source file into an executable
            Switching generators
            Building and linking static and shared libraries
            Controlling compilation with conditionals
            Presenting options to the user
            Specifying the compiler
            Switching the build type
            Controlling compiler flags
            Setting the standard for the language
            Using control flow constructs

- 02. Detecting The Environment
           
            Discovering the operating system
            Dealing with platform-dependent source code
            Dealing with compiler-dependent source code
            Discovering the host processor architecture
            Discovering the host processor instruction set
            Enabling vectorization for the Eigen library

- 03. Detecting External Libraries And Programs
           
            Detecting the Python interpreter
            Detecting the Python library
            Detecting Python modules and packages
            Detecting the BLAS and LAPACK math libraries
            Detecting the OpenMP parallel environment
            Detecting the MPI parallel environment
            Detecting the Eigen library
            Detecting the Boost libraries
            Detecting external libraries: I. Using pkg-config
            Detecting external libraries: II. Writing a find-module

- 04. Creating And Running Tests
           
            Creating a simple unit test
            Defining a unit test using the Catch2 library
            Defining a unit test and linking against Google Test
            Defining a unit test and linking against Boost test
            Using dynamic analysis to detect memory defects
            Testing expected failures
            Using timeouts for long tests
            Running tests in parallel
            Running a subset of tests
            Using test fixtures

- 05. Configure-Time And Build-Time Operations
           
            Using platform-independent file operations
            Running a custom command at configure time
            Running a custom command at build time: I. Using add_custom_command
            Running a custom command at build time: II. Using add_custom_target
            Running custom commands for specific targets at build time
            Probing compilation and linking
            Probing compiler flags
            Probing execution
            Fine-tuning configuration and compilation with generator expressions

- 06. Generating Source Code
           
            Generating sources at configure time
            Generating source code at configure time using Python
            Generating source code at build time using Python
            Recording the project version information for reproducibility
            Recording the project version from a file
            Recording the Git hash at configure time
            Recording the Git hash at build time

- 07. Structuring Projects
           
            Code reuse with functions and macros
            Splitting CMake sources into modules
            Writing a function to test and set compiler flags
            Defining a function or macro with named arguments
            Redefining functions and macros
            Deprecating functions, macros, and variables
            Limiting scope with add_subdirectory
            Avoiding global variables using target_sources
            Organizing Fortran projects

- 08. The Superbuild Pattern
           
            Using the superbuild pattern
            Managing dependencies with a superbuild: I. The Boost libraries
            Managing dependencies with a superbuild: II. The FFTW library
            Managing dependencies with a superbuild: III. The Google Test framework
            Managing your project as a superbuild

- 09.  Mixed-Language Projects
           
            Building Fortran projects that use C/C++ libraries
            Building C/C++ projects that use Fortran libraries
            Building C++ and Python projects using Cython
            Building C++ and Python projects using Boost.Python
            Building C++ and Python projects using pybind11
            Mixing C, C++, Fortran, and Python using Python CFFI

- 10. Writing An Installer
           
            Installing your project
            Installing to standard locations
            Target properties and RPATH handling
            Installation directives
            Generating export headers
            Exporting your targets
            Installing a superbuild

- 11. Packaging Projects
           
            Generating source and binary packages
            Source archives
            Binary archives
            Platform-native binary installers
            Distributing a C++/Python project built with CMake/pybind11 via PyPI
            Distributing a C/Fortran/Python project build with CMake/CFFI via PyPI
            Distributing a simple project as Conda package
            Distributing a project with dependencies as Conda package

- 12. Building Documentation
           
            Building documentation using Doxygen
            Building documentation using Sphinx
            Combining Doxygen and Sphinx

- 13. Alternative Generators And Cross-Compilation
           
            Building a CMake project using Visual Studio 2017
            Cross-compiling a hello world example
            Cross-compiling a Windows binary with OpenMP parallelization

- 14. Testing Dashboards
           
            Setting up a CDash dashboard
            Deploying tests to the CDash dashboard
            Reporting test coverage to the CDash dashboard
            Using the AddressSanitizer and reporting memory defects to CDash
            Using the ThreadSanitizer and reporting data races to CDash

- 15. Porting A Project To CMake

            Where to start
            Reproducing the porting example
            Creating a top-level CMakeLists.txt
            How to allow both conventional configuration and configuration with CMake at the same time
            Capturing a record of what the traditional build does
            Debugging the migration
            Implementing options
            Start with the executable and very few targets, later localize scope
            Generating files and writing platform checks
            How to structure files
            Configuring preprocessor definitions based on the system environment
            Configuring files with paths and compiler flags
            Executing shell scripts at configure time
            Detecting required dependencies and linking
            Reproducing compiler flags
            Defining compiler flags
            Scope of compiler flags
            Porting tests
            Getting started
            Implementing a multi-step test
            Recommendation for tests
            Porting install targets
            Further steps
                  and common pitfalls when converting projects to CMake
