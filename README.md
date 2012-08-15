# reload-modified middleware

The reload-modified middleware automatically reloads namespaces when
their associated source files are modified.

## Installation

Add the following dependency to your `project.clj` file:

    [ring-reload-modified "0.1.2"]

## Example

    (use 'ring.middleware.reload-modified)
    
    (def app
      (wrap-reload-modified #'handler ["src"]))

## Notes on forked version

I took this from https://github.com/weavejester/ring-reload-modified and change it into the last version of Clojure. I change the version tag to 1.1.2 just to make it different with the original one created by James Reeves (https://github.com/weavejester) See the project.clj for more information (bpdp).
