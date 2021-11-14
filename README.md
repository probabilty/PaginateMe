# PaginateMe
efcore pagination automation for c#

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://github.com/probabilty/SELECT/tree/master)

## Features

- Extremly easy to use
- Light weight
- Unify and simplfy Apis
- Multi-platform
- Pure c#
- Opensource
- MIT License


## Installation

Using package manager 
```sh
Install-Package PaginateMe -Version 1.0.1
```
Using DOTNET CLI
```sh
dotnet add package PaginateMe --version 1.0.1
```
Using  PackageReference
```sh
<PackageReference Include="PaginateMe" Version="1.0.1" />
```

## Usage

use it on any Datbase set 

 ```c#
     var pagedModel = await _dbContext.Set
      .OrderByDescending(b => b.Id)
       .PaginateAsync<IBranch>(page, limit);
 ```
 
Where page is the page number, limit is the page size and Set is the model you are working on
