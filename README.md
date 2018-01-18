# letsflow
Re-usable workflows for businesses processes and operations management.

Create a set of related tasks that represent a process within your company.  Save this as a template, and then you can generate those sets of tasks with a single click of a button.

Document how you handle things in your business and make it easier to train new employees.

Commercial license is available.


Directory structure

README.md # overview of system on github.com

Makefile 

package.json # dependencies for Vue JS

client/ #Vue JS see https://vuejs-template.github.io/webpack/structure.html
  build/ # webpack config files
  config/ # main project config
  src/ # js source
  static/ # static assets 
  test/ # js tests
    unit/
    e2e/

server/
  glide.yaml  # dependencies for Go via Glide
  lib/ # Go library code
    controllers/
    models/
    utility/
  main/ # main server code
  test/ # tests generated from Gherkin
  vendor/ # vendored dependencies
  
docs/
  REQUIREMENTS.md # top level requirements in markdown
  features/ # Gherkin features for generating  test stubs
  usermanual/ # User documentation manual in Markdown

