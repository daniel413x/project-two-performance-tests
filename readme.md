# Crag Supply Co. Application Performance Testing

## Repositories

Our repositories: \
https://github.com/brittshook/inventory-mgmt-p1 \
https://github.com/daniel413x/project-two-performance-tests \
https://github.com/daniel413x/project-two-functional-tests

## Info

### Runtime environment

Our performance tests are run on a Jenkins server and facilitated through Taurus via the command:

`bzt "project-two-performance-tests/stepping.yml"`

### Conventions

project-two-performance-tests ***.jmx*** files are named according to the following convention: writing in kebab case, start with the method, e.g. get, post, follow with the *path tested* and suffix with "test plan":

get-api-warehouse-test-plan.jmx <span style="opacity:50%"># http://.../api/warehouse</span>

For simplicity, params and slashes are reduced alike:

get-api-warehouse-1-test-plan.jmx <span style="opacity:50%"># http://.../api/warehouse/1</span> \
get-api-inventory-category-1-test-plan.jmx <span style="opacity:50%"># http://.../api/inventory?category=1</span>

project-two-performance-tests .jmx files are named according to the following convention: start with method e.g. get, post, follow with the *path tested* in snake case:
