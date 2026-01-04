This example Python project presents a suggested project/directory structure
for Python projects that use PyTest for unit testing.  The project is called
'project_01'.

The directory structure is as follows:

my-project/
├── .gitignore
├── pyproject.toml
├── README.md
├── src
│   └── my-package
│       ├── __init__.py
│       ├── module_1.py
│       └── module_2.py
└── tests
    ├── __init__.py
    ├── test_module_1.py
    └── test_module_2.py

.gitignore: Specifies files and directories that should be ignored by Git 
    (e.g., __pycache__, virtual environments, editor configuration files).

pyproject.toml: The modern standard for storing project metadata, 
    dependencies, and configuration for tools like linters and formatters.
    
README.md: Provides essential information about your project, its purpose, 
    and instructions for installation and usage.

src/: Contains the actual Python source code that is part of your main 
    package(s). This approach ensures that developers and users have the same 
    import experience.
    
my_package/: The top-level package directory for your project's code.

    __init__.py: This file tells Python to treat the directory as a package. 
    It can be an empty file, which is a common and good practice for simple 
    packages.
    
    module_1.py, module_2.py: These files (modules) contain your functions, 
    classes, and main application logic.

tests/: Contains unit and integration tests for your code. This is separate 
    from the source code so it doesn't get installed with your package.

