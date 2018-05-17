+++
title = "App Svcs Declare"
date = 2018-05-15T16:35:46-06:00
toc = true
bref = "API docs can be rendered like this one"
+++

## Heading 1

```
https://example.f5.com/some/endpoint
```
  
API endpoint description

### Heading 2


API endpoint usage and examples

```
GET https://example.f5.com/some/endpoint
```

Use the above command to:

- a
- b
- c


## Class: `AppSvcsDeclare`


### Children

#### Description


None

#### Function: `wrapperAjv`

prepare an instance of ajv to validate request payloads. Upon success
leaves ajv instance in this.requestValidator. Throws on error.
this.requestValidator is synchronous; the request schema ignores
declaration contents (which we run through  parser later)

#### Function: `declarationIndex`

list all locally-saved declarations (if any) (relies on caller to set
'this')

#### Function: `savedDeclaration`

return a Promise to obtain the saved declaration (if any) for target +
age. If age is zero and no local copy is available and target seems
reachable, try to get stored declaration from target device.

#### Function: `onDelete`

Attempt to remove one or more tenants when caller uses
DELETE method.

Caller's authorization is not checked here but rather in doTheNeedful().

Member: `WORKER_URI_PATH`:

Member: `isPublic`:

Member: `isPassThrough`:

Member: `isPersisted`:

Member: `isStateRequiredOnStart`:

Member: `requestValidator`:

Member: `myParser`:

Member: `localBigip`:

Member: `controls`:

Member: `state`:

Member: `canSaveState`:
