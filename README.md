# api documentation for  [fantasy-land (v3.2.0)](https://github.com/fantasyland/fantasy-land)  [![npm package](https://img.shields.io/npm/v/npmdoc-fantasy-land.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-fantasy-land) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-fantasy-land.svg)](https://travis-ci.org/npmdoc/node-npmdoc-fantasy-land)
#### Specification for interoperability of common algebraic structures in JavaScript

[![NPM](https://nodei.co/npm/fantasy-land.png?downloads=true)](https://www.npmjs.com/package/fantasy-land)

[![apidoc](https://npmdoc.github.io/node-npmdoc-fantasy-land/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-fantasy-land_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-fantasy-land/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-fantasy-land/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-fantasy-land/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Brian McKenna"
    },
    "bugs": {
        "url": "https://github.com/fantasyland/fantasy-land/issues"
    },
    "dependencies": {
        "daggy": "0.0.x",
        "fantasy-combinators": "0.0.x"
    },
    "description": "Specification for interoperability of common algebraic structures in JavaScript",
    "devDependencies": {
        "eslint": "3.8.x",
        "nodeunit": "0.9.x",
        "sanctuary-style": "0.2.x",
        "xyz": "2.0.x"
    },
    "directories": {},
    "dist": {
        "shasum": "cf9ee50bd96fc1c1562556f9c0363f5ec0ca2cd2",
        "tarball": "https://registry.npmjs.org/fantasy-land/-/fantasy-land-3.2.0.tgz"
    },
    "files": [
        "index.js",
        "internal/*.js",
        "laws/*.js"
    ],
    "gitHead": "a5d90e8520b448835df3cd2f932284353a3f06e6",
    "homepage": "https://github.com/fantasyland/fantasy-land",
    "issues": {
        "url": "https://github.com/fantasyland/fantasy-land/issues"
    },
    "keywords": [
        "algebraic",
        "monad",
        "applicative",
        "functor",
        "monoid",
        "semigroup",
        "chain",
        "apply"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "davidchambers",
            "email": "dc@davidchambers.me"
        },
        {
            "name": "joneshf",
            "email": "jones3.hardy@gmail.com"
        },
        {
            "name": "kennknowles",
            "email": "kenn.knowles@gmail.com"
        },
        {
            "name": "laiff",
            "email": "q.laiff@gmail.com"
        },
        {
            "name": "puffnfresh",
            "email": "brian@brianmckenna.org"
        },
        {
            "name": "stickupkid",
            "email": "stickupkid@gmail.com"
        }
    ],
    "name": "fantasy-land",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/fantasyland/fantasy-land.git"
    },
    "scripts": {
        "lint": "eslint --config node_modules/sanctuary-style/eslint-es6.json --env es6 --env node --rule 'max-len: [off]' -- *.js laws/*.js internal/*.js",
        "release-major": "xyz --repo git@github.com:fantasyland/fantasy-land.git --increment major",
        "release-minor": "xyz --repo git@github.com:fantasyland/fantasy-land.git --increment minor",
        "release-patch": "xyz --repo git@github.com:fantasyland/fantasy-land.git --increment patch",
        "test": "npm run-script lint && npm run-script unit",
        "unit": "nodeunit test.js"
    },
    "version": "3.2.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module fantasy-land](#apidoc.module.fantasy-land)
1.  [function <span class="apidocSignatureSpan">fantasy-land.</span>compose ()](#apidoc.element.fantasy-land.compose)
1.  [function <span class="apidocSignatureSpan">fantasy-land.</span>id ()](#apidoc.element.fantasy-land.id)
1.  [function <span class="apidocSignatureSpan">fantasy-land.</span>string_sum ()](#apidoc.element.fantasy-land.string_sum)
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>alternative
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>applicative
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>apply
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>bifunctor
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>chainrec
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>comonad
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>compose.prototype
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>contravariant
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>foldable
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>func
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>functor
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>id.prototype
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>monad
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>monoid
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>ord
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>plus
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>profunctor
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>semigroup
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>setoid
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>string_sum.prototype
1.  object <span class="apidocSignatureSpan">fantasy-land.</span>traversable
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>alt
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>ap
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>bimap
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>chain
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>chainRec
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>concat
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>contramap
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>empty
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>equals
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>extend
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>extract
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>lte
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>map
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>of
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>promap
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>reduce
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>traverse
1.  string <span class="apidocSignatureSpan">fantasy-land.</span>zero

#### [module fantasy-land.alt](#apidoc.module.fantasy-land.alt)
1.  [function <span class="apidocSignatureSpan">fantasy-land.alt.</span>associativity ( a[alt](b)](#apidoc.element.fantasy-land.alt.associativity)
1.  [function <span class="apidocSignatureSpan">fantasy-land.alt.</span>distributivity ( a[alt](b)](#apidoc.element.fantasy-land.alt.distributivity)

#### [module fantasy-land.alternative](#apidoc.module.fantasy-land.alternative)
1.  [function <span class="apidocSignatureSpan">fantasy-land.alternative.</span>annihilation ( x[ap](T[zero]()](#apidoc.element.fantasy-land.alternative.annihilation)
1.  [function <span class="apidocSignatureSpan">fantasy-land.alternative.</span>distributivity ( x[ap](f[alt](g)](#apidoc.element.fantasy-land.alternative.distributivity)

#### [module fantasy-land.applicative](#apidoc.module.fantasy-land.applicative)
1.  [function <span class="apidocSignatureSpan">fantasy-land.applicative.</span>homomorphism (x)](#apidoc.element.fantasy-land.applicative.homomorphism)
1.  [function <span class="apidocSignatureSpan">fantasy-land.applicative.</span>identity (x)](#apidoc.element.fantasy-land.applicative.identity)
1.  [function <span class="apidocSignatureSpan">fantasy-land.applicative.</span>interchange (identity)](#apidoc.element.fantasy-land.applicative.interchange)

#### [module fantasy-land.apply](#apidoc.module.fantasy-land.apply)
1.  [function <span class="apidocSignatureSpan">fantasy-land.apply.</span>composition (identity)](#apidoc.element.fantasy-land.apply.composition)

#### [module fantasy-land.bifunctor](#apidoc.module.fantasy-land.bifunctor)
1.  [function <span class="apidocSignatureSpan">fantasy-land.bifunctor.</span>composition (x)](#apidoc.element.fantasy-land.bifunctor.composition)
1.  [function <span class="apidocSignatureSpan">fantasy-land.bifunctor.</span>identity (x)](#apidoc.element.fantasy-land.bifunctor.identity)

#### [module fantasy-land.chain](#apidoc.module.fantasy-land.chain)
1.  [function <span class="apidocSignatureSpan">fantasy-land.chain.</span>associativity (x)](#apidoc.element.fantasy-land.chain.associativity)

#### [module fantasy-land.chainrec](#apidoc.module.fantasy-land.chainrec)
1.  [function <span class="apidocSignatureSpan">fantasy-land.chainrec.</span>equivalence ((next, done, v)](#apidoc.element.fantasy-land.chainrec.equivalence)

#### [module fantasy-land.comonad](#apidoc.module.fantasy-land.comonad)
1.  [function <span class="apidocSignatureSpan">fantasy-land.comonad.</span>leftIdentity (x)](#apidoc.element.fantasy-land.comonad.leftIdentity)
1.  [function <span class="apidocSignatureSpan">fantasy-land.comonad.</span>rightIdentity (x)](#apidoc.element.fantasy-land.comonad.rightIdentity)

#### [module fantasy-land.compose](#apidoc.module.fantasy-land.compose)
1.  [function <span class="apidocSignatureSpan">fantasy-land.</span>compose ()](#apidoc.element.fantasy-land.compose.compose)
1.  number <span class="apidocSignatureSpan">fantasy-land.compose.</span>_length

#### [module fantasy-land.compose.prototype](#apidoc.module.fantasy-land.compose.prototype)

#### [module fantasy-land.contravariant](#apidoc.module.fantasy-land.contravariant)
1.  [function <span class="apidocSignatureSpan">fantasy-land.contravariant.</span>composition (x)](#apidoc.element.fantasy-land.contravariant.composition)
1.  [function <span class="apidocSignatureSpan">fantasy-land.contravariant.</span>identity (x)](#apidoc.element.fantasy-land.contravariant.identity)

#### [module fantasy-land.extend](#apidoc.module.fantasy-land.extend)
1.  [function <span class="apidocSignatureSpan">fantasy-land.extend.</span>associativity (x)](#apidoc.element.fantasy-land.extend.associativity)

#### [module fantasy-land.foldable](#apidoc.module.fantasy-land.foldable)
1.  [function <span class="apidocSignatureSpan">fantasy-land.foldable.</span>associativity (x)](#apidoc.element.fantasy-land.foldable.associativity)

#### [module fantasy-land.func](#apidoc.module.fantasy-land.func)
1.  [function <span class="apidocSignatureSpan">fantasy-land.func.</span>equality (x, y)](#apidoc.element.fantasy-land.func.equality)
1.  [function <span class="apidocSignatureSpan">fantasy-land.func.</span>lte (x, y)](#apidoc.element.fantasy-land.func.lte)

#### [module fantasy-land.functor](#apidoc.module.fantasy-land.functor)
1.  [function <span class="apidocSignatureSpan">fantasy-land.functor.</span>composition (x)](#apidoc.element.fantasy-land.functor.composition)
1.  [function <span class="apidocSignatureSpan">fantasy-land.functor.</span>identity (x)](#apidoc.element.fantasy-land.functor.identity)

#### [module fantasy-land.id](#apidoc.module.fantasy-land.id)
1.  [function <span class="apidocSignatureSpan">fantasy-land.</span>id ()](#apidoc.element.fantasy-land.id.id)
1.  number <span class="apidocSignatureSpan">fantasy-land.id.</span>_length

#### [module fantasy-land.id.prototype](#apidoc.module.fantasy-land.id.prototype)
1.  [function <span class="apidocSignatureSpan">fantasy-land.id.prototype.</span>toArray ()](#apidoc.element.fantasy-land.id.prototype.toArray)

#### [module fantasy-land.monad](#apidoc.module.fantasy-land.monad)
1.  [function <span class="apidocSignatureSpan">fantasy-land.monad.</span>leftIdentity (x)](#apidoc.element.fantasy-land.monad.leftIdentity)
1.  [function <span class="apidocSignatureSpan">fantasy-land.monad.</span>rightIdentity (x)](#apidoc.element.fantasy-land.monad.rightIdentity)

#### [module fantasy-land.monoid](#apidoc.module.fantasy-land.monoid)
1.  [function <span class="apidocSignatureSpan">fantasy-land.monoid.</span>leftIdentity ()](#apidoc.element.fantasy-land.monoid.leftIdentity)
1.  [function <span class="apidocSignatureSpan">fantasy-land.monoid.</span>rightIdentity (x)](#apidoc.element.fantasy-land.monoid.rightIdentity)

#### [module fantasy-land.ord](#apidoc.module.fantasy-land.ord)
1.  [function <span class="apidocSignatureSpan">fantasy-land.ord.</span>antisymmetry (g)](#apidoc.element.fantasy-land.ord.antisymmetry)
1.  [function <span class="apidocSignatureSpan">fantasy-land.ord.</span>totality (g)](#apidoc.element.fantasy-land.ord.totality)
1.  [function <span class="apidocSignatureSpan">fantasy-land.ord.</span>transitivity (g)](#apidoc.element.fantasy-land.ord.transitivity)

#### [module fantasy-land.plus](#apidoc.module.fantasy-land.plus)
1.  [function <span class="apidocSignatureSpan">fantasy-land.plus.</span>annihilation ( T[zero]()](#apidoc.element.fantasy-land.plus.annihilation)
1.  [function <span class="apidocSignatureSpan">fantasy-land.plus.</span>leftIdentity ( x[alt](T[zero]()](#apidoc.element.fantasy-land.plus.leftIdentity)
1.  [function <span class="apidocSignatureSpan">fantasy-land.plus.</span>rightIdentity ( T[zero]()](#apidoc.element.fantasy-land.plus.rightIdentity)

#### [module fantasy-land.profunctor](#apidoc.module.fantasy-land.profunctor)
1.  [function <span class="apidocSignatureSpan">fantasy-land.profunctor.</span>composition (x)](#apidoc.element.fantasy-land.profunctor.composition)
1.  [function <span class="apidocSignatureSpan">fantasy-land.profunctor.</span>identity (x)](#apidoc.element.fantasy-land.profunctor.identity)

#### [module fantasy-land.semigroup](#apidoc.module.fantasy-land.semigroup)
1.  [function <span class="apidocSignatureSpan">fantasy-land.semigroup.</span>associativity (x)](#apidoc.element.fantasy-land.semigroup.associativity)

#### [module fantasy-land.setoid](#apidoc.module.fantasy-land.setoid)
1.  [function <span class="apidocSignatureSpan">fantasy-land.setoid.</span>reflexivity (x)](#apidoc.element.fantasy-land.setoid.reflexivity)
1.  [function <span class="apidocSignatureSpan">fantasy-land.setoid.</span>symmetry (x)](#apidoc.element.fantasy-land.setoid.symmetry)
1.  [function <span class="apidocSignatureSpan">fantasy-land.setoid.</span>transitivity (x)](#apidoc.element.fantasy-land.setoid.transitivity)

#### [module fantasy-land.string_sum](#apidoc.module.fantasy-land.string_sum)
1.  [function <span class="apidocSignatureSpan">fantasy-land.</span>string_sum ()](#apidoc.element.fantasy-land.string_sum.string_sum)
1.  number <span class="apidocSignatureSpan">fantasy-land.string_sum.</span>_length

#### [module fantasy-land.string_sum.prototype](#apidoc.module.fantasy-land.string_sum.prototype)

#### [module fantasy-land.traversable](#apidoc.module.fantasy-land.traversable)
1.  [function <span class="apidocSignatureSpan">fantasy-land.traversable.</span>composition (x)](#apidoc.element.fantasy-land.traversable.composition)
1.  [function <span class="apidocSignatureSpan">fantasy-land.traversable.</span>identity (T, T[of])](#apidoc.element.fantasy-land.traversable.identity)
1.  [function <span class="apidocSignatureSpan">fantasy-land.traversable.</span>naturality (t(x)](#apidoc.element.fantasy-land.traversable.naturality)



# <a name="apidoc.module.fantasy-land"></a>[module fantasy-land](#apidoc.module.fantasy-land)

#### <a name="apidoc.element.fantasy-land.compose"></a>[function <span class="apidocSignatureSpan">fantasy-land.</span>compose ()](#apidoc.element.fantasy-land.compose)
- description and source-code
```javascript
function wrapped() {
    var self = getInstance(this, wrapped),
        i;

    if(arguments.length != fields.length)
        throw new TypeError('Expected ' + fields.length + ' arguments, got ' + arguments.length);

    for(i = 0; i < fields.length; i++)
        self[fields[i]] = arguments[i];

    return self;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.id"></a>[function <span class="apidocSignatureSpan">fantasy-land.</span>id ()](#apidoc.element.fantasy-land.id)
- description and source-code
```javascript
function wrapped() {
    var self = getInstance(this, wrapped),
        i;

    if(arguments.length != fields.length)
        throw new TypeError('Expected ' + fields.length + ' arguments, got ' + arguments.length);

    for(i = 0; i < fields.length; i++)
        self[fields[i]] = arguments[i];

    return self;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.string_sum"></a>[function <span class="apidocSignatureSpan">fantasy-land.</span>string_sum ()](#apidoc.element.fantasy-land.string_sum)
- description and source-code
```javascript
function wrapped() {
    var self = getInstance(this, wrapped),
        i;

    if(arguments.length != fields.length)
        throw new TypeError('Expected ' + fields.length + ' arguments, got ' + arguments.length);

    for(i = 0; i < fields.length; i++)
        self[fields[i]] = arguments[i];

    return self;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.alt"></a>[module fantasy-land.alt](#apidoc.module.fantasy-land.alt)

#### <a name="apidoc.element.fantasy-land.alt.associativity"></a>[function <span class="apidocSignatureSpan">fantasy-land.alt.</span>associativity ( a[alt](b)](#apidoc.element.fantasy-land.alt.associativity)
- description and source-code
```javascript
eq => a => b => c => eq( a[alt](b)[alt](c),
  a[alt](b[alt](c))
)
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.alt.distributivity"></a>[function <span class="apidocSignatureSpan">fantasy-land.alt.</span>distributivity ( a[alt](b)](#apidoc.element.fantasy-land.alt.distributivity)
- description and source-code
```javascript
eq => a => b => f => eq( a[alt](b)[map](f),
  a[map](f)[alt](b[map](f))
)
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.alternative"></a>[module fantasy-land.alternative](#apidoc.module.fantasy-land.alternative)

#### <a name="apidoc.element.fantasy-land.alternative.annihilation"></a>[function <span class="apidocSignatureSpan">fantasy-land.alternative.</span>annihilation ( x[ap](T[zero]()](#apidoc.element.fantasy-land.alternative.annihilation)
- description and source-code
```javascript
T => eq => x => eq( x[ap](T[zero]()),
  T[zero]()
)
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.alternative.distributivity"></a>[function <span class="apidocSignatureSpan">fantasy-land.alternative.</span>distributivity ( x[ap](f[alt](g)](#apidoc.element.fantasy-land.alternative.distributivity)
- description and source-code
```javascript
eq => x => f => g => eq( x[ap](f[alt](g)),
  x[ap](f)[alt](x[ap](g))
)
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.applicative"></a>[module fantasy-land.applicative](#apidoc.module.fantasy-land.applicative)

#### <a name="apidoc.element.fantasy-land.applicative.homomorphism"></a>[function <span class="apidocSignatureSpan">fantasy-land.applicative.</span>homomorphism (x)](#apidoc.element.fantasy-land.applicative.homomorphism)
- description and source-code
```javascript
T => eq => x => {
  const a = T[of](x)[ap](T[of](identity));
  const b = T[of](identity(x));
  return eq(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.applicative.identity"></a>[function <span class="apidocSignatureSpan">fantasy-land.applicative.</span>identity (x)](#apidoc.element.fantasy-land.applicative.identity)
- description and source-code
```javascript
T => eq => x => {
  const a = T[of](x)[ap](T[of](identity));
  const b = T[of](x);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.applicative.interchange"></a>[function <span class="apidocSignatureSpan">fantasy-land.applicative.</span>interchange (identity)](#apidoc.element.fantasy-land.applicative.interchange)
- description and source-code
```javascript
T => eq => x => {
  const u = T[of](identity);

  const a = T[of](x)[ap](u);
  const b = u[ap](T[of](thrush(x)));
  return eq(a, b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.apply"></a>[module fantasy-land.apply](#apidoc.module.fantasy-land.apply)

#### <a name="apidoc.element.fantasy-land.apply.composition"></a>[function <span class="apidocSignatureSpan">fantasy-land.apply.</span>composition (identity)](#apidoc.element.fantasy-land.apply.composition)
- description and source-code
```javascript
t => eq => x => {
  const y = t[of](identity);

  const a = y[ap](y[ap](y[map](compose)));
  const b = y[ap](y)[ap](y);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.bifunctor"></a>[module fantasy-land.bifunctor](#apidoc.module.fantasy-land.bifunctor)

#### <a name="apidoc.element.fantasy-land.bifunctor.composition"></a>[function <span class="apidocSignatureSpan">fantasy-land.bifunctor.</span>composition (x)](#apidoc.element.fantasy-land.bifunctor.composition)
- description and source-code
```javascript
t => eq => x => {
  const a = t(x)[bimap](compose(identity)(identity), compose(identity)(identity));
  const b = t(x)[bimap](identity, identity)[bimap](identity, identity);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.bifunctor.identity"></a>[function <span class="apidocSignatureSpan">fantasy-land.bifunctor.</span>identity (x)](#apidoc.element.fantasy-land.bifunctor.identity)
- description and source-code
```javascript
t => eq => x => {
  const a = t(x)[bimap](identity, identity);
  const b = t(x);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.chain"></a>[module fantasy-land.chain](#apidoc.module.fantasy-land.chain)

#### <a name="apidoc.element.fantasy-land.chain.associativity"></a>[function <span class="apidocSignatureSpan">fantasy-land.chain.</span>associativity (x)](#apidoc.element.fantasy-land.chain.associativity)
- description and source-code
```javascript
t => eq => x => {
  const a = t[of](x)[chain](t[of])[chain](t[of]);
  const b = t[of](x)[chain](x => t[of](x)[chain](t[of]));
  return eq(a, b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.chainrec"></a>[module fantasy-land.chainrec](#apidoc.module.fantasy-land.chainrec)

#### <a name="apidoc.element.fantasy-land.chainrec.equivalence"></a>[function <span class="apidocSignatureSpan">fantasy-land.chainrec.</span>equivalence ((next, done, v)](#apidoc.element.fantasy-land.chainrec.equivalence)
- description and source-code
```javascript
T => eq => p => d => n => x => {
  const a = T[chainRec]((next, done, v) => p(v) ? d(v)[map](done) : n(v)[map](next), x);
  const b = (function step(v) { return p(v) ? d(v) : n(v)[chain](step); }(x));
  return eq(a, b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.comonad"></a>[module fantasy-land.comonad](#apidoc.module.fantasy-land.comonad)

#### <a name="apidoc.element.fantasy-land.comonad.leftIdentity"></a>[function <span class="apidocSignatureSpan">fantasy-land.comonad.</span>leftIdentity (x)](#apidoc.element.fantasy-land.comonad.leftIdentity)
- description and source-code
```javascript
t => eq => x => {
  const a = t(x)[extend](identity)[extract]();
  const b = t(x);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.comonad.rightIdentity"></a>[function <span class="apidocSignatureSpan">fantasy-land.comonad.</span>rightIdentity (x)](#apidoc.element.fantasy-land.comonad.rightIdentity)
- description and source-code
```javascript
t => eq => x => {
  const a = t(x)[extend](w => w[extract]());
  const b = t(x);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.compose"></a>[module fantasy-land.compose](#apidoc.module.fantasy-land.compose)

#### <a name="apidoc.element.fantasy-land.compose.compose"></a>[function <span class="apidocSignatureSpan">fantasy-land.</span>compose ()](#apidoc.element.fantasy-land.compose.compose)
- description and source-code
```javascript
function wrapped() {
    var self = getInstance(this, wrapped),
        i;

    if(arguments.length != fields.length)
        throw new TypeError('Expected ' + fields.length + ' arguments, got ' + arguments.length);

    for(i = 0; i < fields.length; i++)
        self[fields[i]] = arguments[i];

    return self;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.compose.prototype"></a>[module fantasy-land.compose.prototype](#apidoc.module.fantasy-land.compose.prototype)



# <a name="apidoc.module.fantasy-land.contravariant"></a>[module fantasy-land.contravariant](#apidoc.module.fantasy-land.contravariant)

#### <a name="apidoc.element.fantasy-land.contravariant.composition"></a>[function <span class="apidocSignatureSpan">fantasy-land.contravariant.</span>composition (x)](#apidoc.element.fantasy-land.contravariant.composition)
- description and source-code
```javascript
t => eq => x => {
  const a = t(x)[contramap](compose(identity)(identity));
  const b = t(x)[contramap](identity)[contramap](identity);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.contravariant.identity"></a>[function <span class="apidocSignatureSpan">fantasy-land.contravariant.</span>identity (x)](#apidoc.element.fantasy-land.contravariant.identity)
- description and source-code
```javascript
t => eq => x => {
  const a = t(x)[contramap](identity);
  const b = t(x);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.extend"></a>[module fantasy-land.extend](#apidoc.module.fantasy-land.extend)

#### <a name="apidoc.element.fantasy-land.extend.associativity"></a>[function <span class="apidocSignatureSpan">fantasy-land.extend.</span>associativity (x)](#apidoc.element.fantasy-land.extend.associativity)
- description and source-code
```javascript
t => eq => x => {
  const a = t(x)[extend](identity)[extend](identity);
  const b = t(x)[extend](w => identity(w[extend](identity)));
  return eq(a, b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.foldable"></a>[module fantasy-land.foldable](#apidoc.module.fantasy-land.foldable)

#### <a name="apidoc.element.fantasy-land.foldable.associativity"></a>[function <span class="apidocSignatureSpan">fantasy-land.foldable.</span>associativity (x)](#apidoc.element.fantasy-land.foldable.associativity)
- description and source-code
```javascript
t => eq => x => {
  const a = t(x)[reduce](identity, x);
  const b = t(x).toArray()[reduce](identity, x);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.func"></a>[module fantasy-land.func](#apidoc.module.fantasy-land.func)

#### <a name="apidoc.element.fantasy-land.func.equality"></a>[function <span class="apidocSignatureSpan">fantasy-land.func.</span>equality (x, y)](#apidoc.element.fantasy-land.func.equality)
- description and source-code
```javascript
(x, y) => typeof x[fl.equals] === 'function' ? x[fl.equals](y) : x === y
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.func.lte"></a>[function <span class="apidocSignatureSpan">fantasy-land.func.</span>lte (x, y)](#apidoc.element.fantasy-land.func.lte)
- description and source-code
```javascript
(x, y) => {
  if (typeof y[fl.lte] === 'function') return y[fl.lte](x);

  const typeX = typeof x;
  const typeY = typeof y;
  return typeX === typeY && (typeX === 'string' || typeX === 'number') && x <= y;
}
```
- example usage
```shell
...
2. 'equals' must return a boolean ('true' or 'false').

### Ord

A value that implements the Ord specification must also implement
the [Setoid](#setoid) specification.

1. 'a.lte(b)' or 'b.lte(a)' (totality)
2. If 'a.lte(b)' and 'b.lte(a)', then 'a.equals(b)' (antisymmetry)
3. If 'a.lte(b)' and 'b.lte(c)', then 'a.lte(c)' (transitivity)

#### 'lte' method

'''hs
lte :: Ord a => a ~> a -> Boolean
...
```



# <a name="apidoc.module.fantasy-land.functor"></a>[module fantasy-land.functor](#apidoc.module.fantasy-land.functor)

#### <a name="apidoc.element.fantasy-land.functor.composition"></a>[function <span class="apidocSignatureSpan">fantasy-land.functor.</span>composition (x)](#apidoc.element.fantasy-land.functor.composition)
- description and source-code
```javascript
of => eq => f => g => x => {
  const a = of(x)[map](x => f(g(x)));
  const b = of(x)[map](g)[map](f);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.functor.identity"></a>[function <span class="apidocSignatureSpan">fantasy-land.functor.</span>identity (x)](#apidoc.element.fantasy-land.functor.identity)
- description and source-code
```javascript
of => eq => x => {
  const a = of(x)[map](x => x);
  const b = of(x);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.id"></a>[module fantasy-land.id](#apidoc.module.fantasy-land.id)

#### <a name="apidoc.element.fantasy-land.id.id"></a>[function <span class="apidocSignatureSpan">fantasy-land.</span>id ()](#apidoc.element.fantasy-land.id.id)
- description and source-code
```javascript
function wrapped() {
    var self = getInstance(this, wrapped),
        i;

    if(arguments.length != fields.length)
        throw new TypeError('Expected ' + fields.length + ' arguments, got ' + arguments.length);

    for(i = 0; i < fields.length; i++)
        self[fields[i]] = arguments[i];

    return self;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.id.prototype"></a>[module fantasy-land.id.prototype](#apidoc.module.fantasy-land.id.prototype)

#### <a name="apidoc.element.fantasy-land.id.prototype.toArray"></a>[function <span class="apidocSignatureSpan">fantasy-land.id.prototype.</span>toArray ()](#apidoc.element.fantasy-land.id.prototype.toArray)
- description and source-code
```javascript
toArray = function () {
  return [this.value];
}
```
- example usage
```shell
...
const {identity} = require('fantasy-combinators');
const {reduce} = require('..');

/**

### Foldable

1. 'u.reduce' is equivalent to 'u.toArray().reduce'

**/

const associativity = t => eq => x => {
const a = t(x)[reduce](identity, x);
const b = t(x).toArray()[reduce](identity, x);
return eq(a, b);
...
```



# <a name="apidoc.module.fantasy-land.monad"></a>[module fantasy-land.monad](#apidoc.module.fantasy-land.monad)

#### <a name="apidoc.element.fantasy-land.monad.leftIdentity"></a>[function <span class="apidocSignatureSpan">fantasy-land.monad.</span>leftIdentity (x)](#apidoc.element.fantasy-land.monad.leftIdentity)
- description and source-code
```javascript
t => eq => f => x => {
  const a = t[of](x)[chain](f);
  const b = f(x);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.monad.rightIdentity"></a>[function <span class="apidocSignatureSpan">fantasy-land.monad.</span>rightIdentity (x)](#apidoc.element.fantasy-land.monad.rightIdentity)
- description and source-code
```javascript
t => eq => x => {
  const a = t[of](x)[chain](t[of]);
  const b = t[of](x);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.monoid"></a>[module fantasy-land.monoid](#apidoc.module.fantasy-land.monoid)

#### <a name="apidoc.element.fantasy-land.monoid.leftIdentity"></a>[function <span class="apidocSignatureSpan">fantasy-land.monoid.</span>leftIdentity ()](#apidoc.element.fantasy-land.monoid.leftIdentity)
- description and source-code
```javascript
T => eq => x => {
  const a = T[empty]()[concat](T[of](x));
  const b = T[of](x);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.monoid.rightIdentity"></a>[function <span class="apidocSignatureSpan">fantasy-land.monoid.</span>rightIdentity (x)](#apidoc.element.fantasy-land.monoid.rightIdentity)
- description and source-code
```javascript
T => eq => x => {
  const a = T[of](x)[concat](T[empty]());
  const b = T[of](x);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.ord"></a>[module fantasy-land.ord](#apidoc.module.fantasy-land.ord)

#### <a name="apidoc.element.fantasy-land.ord.antisymmetry"></a>[function <span class="apidocSignatureSpan">fantasy-land.ord.</span>antisymmetry (g)](#apidoc.element.fantasy-land.ord.antisymmetry)
- description and source-code
```javascript
eq => f => g => {
  const a = f[lte](g);
  const b = g[lte](f);
  const c = f[equals](g);
  const d = true;
  return eq(a, d) && eq(b, d) && eq(c, d);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.ord.totality"></a>[function <span class="apidocSignatureSpan">fantasy-land.ord.</span>totality (g)](#apidoc.element.fantasy-land.ord.totality)
- description and source-code
```javascript
eq => f => g => {
  const a = f[lte](g);
  const b = g[lte](f);
  const c = true;
  return eq(a || b, c);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.ord.transitivity"></a>[function <span class="apidocSignatureSpan">fantasy-land.ord.</span>transitivity (g)](#apidoc.element.fantasy-land.ord.transitivity)
- description and source-code
```javascript
eq => f => g => h => {
  const a = f[lte](g);
  const b = g[lte](h);
  const c = f[lte](h);
  const d = true;
  return eq(a, d) && eq(b, d) && eq(c, d);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.plus"></a>[module fantasy-land.plus](#apidoc.module.fantasy-land.plus)

#### <a name="apidoc.element.fantasy-land.plus.annihilation"></a>[function <span class="apidocSignatureSpan">fantasy-land.plus.</span>annihilation ( T[zero]()](#apidoc.element.fantasy-land.plus.annihilation)
- description and source-code
```javascript
T => eq => f => eq( T[zero]()[map](f),
  T[zero]()
)
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.plus.leftIdentity"></a>[function <span class="apidocSignatureSpan">fantasy-land.plus.</span>leftIdentity ( x[alt](T[zero]()](#apidoc.element.fantasy-land.plus.leftIdentity)
- description and source-code
```javascript
T => eq => x => eq( x[alt](T[zero]()),
  x
)
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.plus.rightIdentity"></a>[function <span class="apidocSignatureSpan">fantasy-land.plus.</span>rightIdentity ( T[zero]()](#apidoc.element.fantasy-land.plus.rightIdentity)
- description and source-code
```javascript
T => eq => x => eq( T[zero]()[alt](x),
  x
)
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.profunctor"></a>[module fantasy-land.profunctor](#apidoc.module.fantasy-land.profunctor)

#### <a name="apidoc.element.fantasy-land.profunctor.composition"></a>[function <span class="apidocSignatureSpan">fantasy-land.profunctor.</span>composition (x)](#apidoc.element.fantasy-land.profunctor.composition)
- description and source-code
```javascript
t => eq => x => {
  const a = t(x)[promap](compose(identity)(identity), compose(identity)(identity));
  const b = t(x)[promap](identity, identity)[promap](identity, identity);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.profunctor.identity"></a>[function <span class="apidocSignatureSpan">fantasy-land.profunctor.</span>identity (x)](#apidoc.element.fantasy-land.profunctor.identity)
- description and source-code
```javascript
t => eq => x => {
  const a = t(x)[promap](identity, identity);
  const b = t(x);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.semigroup"></a>[module fantasy-land.semigroup](#apidoc.module.fantasy-land.semigroup)

#### <a name="apidoc.element.fantasy-land.semigroup.associativity"></a>[function <span class="apidocSignatureSpan">fantasy-land.semigroup.</span>associativity (x)](#apidoc.element.fantasy-land.semigroup.associativity)
- description and source-code
```javascript
t => eq => x => {
  const f = t(x);
  const g = t(x);
  const h = t(x);

  const a = f[concat](g)[concat](h);
  const b = f[concat](g[concat](h));
  return eq(a, b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.setoid"></a>[module fantasy-land.setoid](#apidoc.module.fantasy-land.setoid)

#### <a name="apidoc.element.fantasy-land.setoid.reflexivity"></a>[function <span class="apidocSignatureSpan">fantasy-land.setoid.</span>reflexivity (x)](#apidoc.element.fantasy-land.setoid.reflexivity)
- description and source-code
```javascript
t => eq => x => {
  const y = t(x);

  const a = y[equals](y);
  const b = true;
  return eq(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.setoid.symmetry"></a>[function <span class="apidocSignatureSpan">fantasy-land.setoid.</span>symmetry (x)](#apidoc.element.fantasy-land.setoid.symmetry)
- description and source-code
```javascript
t => eq => x => {
  const f = t(x);
  const g = t(x);

  const a = f[equals](g);
  const b = g[equals](f);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.setoid.transitivity"></a>[function <span class="apidocSignatureSpan">fantasy-land.setoid.</span>transitivity (x)](#apidoc.element.fantasy-land.setoid.transitivity)
- description and source-code
```javascript
t => eq => x => {
  const f = t(x);
  const g = t(x);
  const h = t(x);

  const a = f[equals](g);
  const b = g[equals](h);
  const c = f[equals](h);
  return eq(a && b, c);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.string_sum"></a>[module fantasy-land.string_sum](#apidoc.module.fantasy-land.string_sum)

#### <a name="apidoc.element.fantasy-land.string_sum.string_sum"></a>[function <span class="apidocSignatureSpan">fantasy-land.</span>string_sum ()](#apidoc.element.fantasy-land.string_sum.string_sum)
- description and source-code
```javascript
function wrapped() {
    var self = getInstance(this, wrapped),
        i;

    if(arguments.length != fields.length)
        throw new TypeError('Expected ' + fields.length + ' arguments, got ' + arguments.length);

    for(i = 0; i < fields.length; i++)
        self[fields[i]] = arguments[i];

    return self;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fantasy-land.string_sum.prototype"></a>[module fantasy-land.string_sum.prototype](#apidoc.module.fantasy-land.string_sum.prototype)



# <a name="apidoc.module.fantasy-land.traversable"></a>[module fantasy-land.traversable](#apidoc.module.fantasy-land.traversable)

#### <a name="apidoc.element.fantasy-land.traversable.composition"></a>[function <span class="apidocSignatureSpan">fantasy-land.traversable.</span>composition (x)](#apidoc.element.fantasy-land.traversable.composition)
- description and source-code
```javascript
T => t => eq => x => {
  const a = t(x)[traverse](Compose, Compose);
  const b = Compose(t(x)[traverse](Id, y => y)[map](x => x[traverse](Id, y => y)));
  return eq(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.traversable.identity"></a>[function <span class="apidocSignatureSpan">fantasy-land.traversable.</span>identity (T, T[of])](#apidoc.element.fantasy-land.traversable.identity)
- description and source-code
```javascript
T => eq => x => {
  const u = [x];

  const a = u[traverse](T, T[of]);
  const b = T[of](u);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fantasy-land.traversable.naturality"></a>[function <span class="apidocSignatureSpan">fantasy-land.traversable.</span>naturality (t(x)](#apidoc.element.fantasy-land.traversable.naturality)
- description and source-code
```javascript
T => t => eq => x => {
  const a = identity(t(x)[traverse](T, y => y));
  const b = t(x)[traverse](T, identity);
  return eq(a, b);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
