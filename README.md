# NodeBB: API

Additional API methods. This plugin depends on write-api plugin.

![Version](https://img.shields.io/npm/v/nodebb-plugin-ns-api.svg)
![Dependencies](https://david-dm.org/NicolasSiver/nodebb-plugin-ns-api.svg)
![bitHound Score](https://www.bithound.io/github/NicolasSiver/nodebb-plugin-ns-api/badges/score.svg)
![Code Climate](https://img.shields.io/codeclimate/github/NicolasSiver/nodebb-plugin-ns-api.svg)

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 

- [Usage](#usage)
- [API](#api)
  - [/api/v1/users/:uid](#apiv1usersuid)
  - [/api/v1/users/:uid/groups](#apiv1usersuidgroups)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Usage

In order to use these extended api methods, you should have [Write Api Plugin](https://github.com/NodeBB/nodebb-plugin-write-api) in your system: activated and configured for token use.

## API

### /api/v1/users/:uid

Profile full data-set about the user

**Result:**

    {
        user data
    }

### /api/v1/users/:uid/groups

Provides all groups to which user belongs.

**Result:**
 
    {
        user: {mini profile of the user},
        groups: [groups collection]
    }    
