# steps to properly clone the project with submodules:

git clone --recurse-submodules https://github.com/chandudammalapati/dummy-multi-main-repo.git

If above step is missed do the below steps: goto main folder path
    
    git submodule init
    
    git submodule update

# steps to add submodule
git submodule add https://github.com/chandudammalapati/second-imported-module.git

# To get latest code from submodule:

git submodule update --remote

    git add .

    git commit -m "commit message says that you fetched all submodule changes"

    git push

or else to go to individual path
git pull
 go to main submodule path 

    git add .

    git commit -m "commit message says that you fetched particular submodule changes"

    git push


# to get a particular branch reference like below:

Now, all the -b does is add one line in your .gitmodules file. So following the same example, it would look like this:
  
  
  [submodule "second-imported-module"]
	path = second-imported-module
	url = https://github.com/chandudammalapati/second-imported-module.git
   branch = dev


# MultiMainRepo

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 11.0.5.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
