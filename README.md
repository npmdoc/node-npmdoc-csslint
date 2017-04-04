# api documentation for  [csslint (v1.0.5)](http://csslint.net/)  [![npm package](https://img.shields.io/npm/v/npmdoc-csslint.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-csslint) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-csslint.svg)](https://travis-ci.org/npmdoc/node-npmdoc-csslint)
#### CSSLint

[![NPM](https://nodei.co/npm/csslint.png?downloads=true)](https://www.npmjs.com/package/csslint)

[![apidoc](https://npmdoc.github.io/node-npmdoc-csslint/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-csslint_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-csslint/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-csslint/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-csslint/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Nicole Sullivan"
    },
    "bin": {
        "csslint": "./dist/cli.js"
    },
    "bugs": {
        "url": "https://github.com/CSSLint/csslint/issues"
    },
    "contributors": [
        {
            "name": "Nicholas C. Zakas"
        }
    ],
    "dependencies": {
        "clone": "~2.1.0",
        "parserlib": "~1.1.1"
    },
    "description": "CSSLint",
    "devDependencies": {
        "grunt": "~1.0.1",
        "grunt-contrib-clean": "~1.0.0",
        "grunt-contrib-concat": "~1.0.0",
        "grunt-contrib-jshint": "~1.1.0",
        "grunt-contrib-watch": "~1.0.0",
        "grunt-include-replace": "~5.0.0",
        "load-grunt-tasks": "~3.5.0",
        "time-grunt": "~1.4.0",
        "yuitest": "~0.7.9"
    },
    "directories": {},
    "dist": {
        "shasum": "19cc3eda322160fd3f7232af1cb2a360e898a2e9",
        "tarball": "https://registry.npmjs.org/csslint/-/csslint-1.0.5.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "files": [
        "dist/cli.js",
        "dist/csslint-node.js",
        "dist/csslint.js",
        "CHANGELOG",
        "LICENSE"
    ],
    "gitHead": "f57c84cf8c202828ae024a4d3ea08f4adceb187a",
    "homepage": "http://csslint.net/",
    "license": "MIT",
    "main": "./dist/csslint-node.js",
    "maintainers": [
        {
            "name": "cscott",
            "email": "cscott@cscott.net"
        },
        {
            "name": "nschonni",
            "email": "nschonni@gmail.com"
        },
        {
            "name": "nzakas",
            "email": "nicholas@nczconsulting.com"
        },
        {
            "name": "stubbornella",
            "email": "nicole@stubbornella.org"
        },
        {
            "name": "xhmikosr",
            "email": "xhmikosr@gmail.com"
        }
    ],
    "name": "csslint",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/CSSLint/csslint.git"
    },
    "scripts": {
        "test": "grunt test"
    },
    "version": "1.0.5"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module csslint](#apidoc.module.csslint)
1.  [function <span class="apidocSignatureSpan">csslint.</span>CSSLint._Reporter (lines, ruleset, allow, ignore)](#apidoc.element.csslint.CSSLint._Reporter)
1.  object <span class="apidocSignatureSpan">csslint.</span>CSSLint
1.  object <span class="apidocSignatureSpan">csslint.</span>CSSLint.Util
1.  object <span class="apidocSignatureSpan">csslint.</span>CSSLint._Reporter.prototype

#### [module csslint.CSSLint](#apidoc.module.csslint.CSSLint)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint.</span>_Reporter (lines, ruleset, allow, ignore)](#apidoc.element.csslint.CSSLint._Reporter)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint.</span>addFormatter (formatter)](#apidoc.element.csslint.CSSLint.addFormatter)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint.</span>addRule (rule)](#apidoc.element.csslint.CSSLint.addRule)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint.</span>clearRules ()](#apidoc.element.csslint.CSSLint.clearRules)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint.</span>format (results, filename, formatId, options)](#apidoc.element.csslint.CSSLint.format)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint.</span>getFormatter (formatId)](#apidoc.element.csslint.CSSLint.getFormatter)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint.</span>getRules ()](#apidoc.element.csslint.CSSLint.getRules)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint.</span>getRuleset ()](#apidoc.element.csslint.CSSLint.getRuleset)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint.</span>hasFormat (formatId)](#apidoc.element.csslint.CSSLint.hasFormat)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint.</span>verify (text, ruleset)](#apidoc.element.csslint.CSSLint.verify)
1.  object <span class="apidocSignatureSpan">csslint.CSSLint.</span>Util
1.  object <span class="apidocSignatureSpan">csslint.CSSLint.</span>_listeners
1.  string <span class="apidocSignatureSpan">csslint.CSSLint.</span>version

#### [module csslint.CSSLint.Util](#apidoc.module.csslint.CSSLint.Util)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint.Util.</span>forEach (values, func)](#apidoc.element.csslint.CSSLint.Util.forEach)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint.Util.</span>indexOf (values, value)](#apidoc.element.csslint.CSSLint.Util.indexOf)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint.Util.</span>mix (receiver, supplier)](#apidoc.element.csslint.CSSLint.Util.mix)

#### [module csslint.CSSLint._Reporter](#apidoc.module.csslint.CSSLint._Reporter)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint.</span>_Reporter (lines, ruleset, allow, ignore)](#apidoc.element.csslint.CSSLint._Reporter._Reporter)

#### [module csslint.CSSLint._Reporter.prototype](#apidoc.module.csslint.CSSLint._Reporter.prototype)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint._Reporter.prototype.</span>constructor (lines, ruleset, allow, ignore)](#apidoc.element.csslint.CSSLint._Reporter.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint._Reporter.prototype.</span>error (message, line, col, rule)](#apidoc.element.csslint.CSSLint._Reporter.prototype.error)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint._Reporter.prototype.</span>info (message, line, col, rule)](#apidoc.element.csslint.CSSLint._Reporter.prototype.info)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint._Reporter.prototype.</span>report (message, line, col, rule)](#apidoc.element.csslint.CSSLint._Reporter.prototype.report)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint._Reporter.prototype.</span>rollupError (message, rule)](#apidoc.element.csslint.CSSLint._Reporter.prototype.rollupError)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint._Reporter.prototype.</span>rollupWarn (message, rule)](#apidoc.element.csslint.CSSLint._Reporter.prototype.rollupWarn)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint._Reporter.prototype.</span>stat (name, value)](#apidoc.element.csslint.CSSLint._Reporter.prototype.stat)
1.  [function <span class="apidocSignatureSpan">csslint.CSSLint._Reporter.prototype.</span>warn (message, line, col, rule)](#apidoc.element.csslint.CSSLint._Reporter.prototype.warn)



# <a name="apidoc.module.csslint"></a>[module csslint](#apidoc.module.csslint)

#### <a name="apidoc.element.csslint.CSSLint._Reporter"></a>[function <span class="apidocSignatureSpan">csslint.</span>CSSLint._Reporter (lines, ruleset, allow, ignore)](#apidoc.element.csslint.CSSLint._Reporter)
- description and source-code
```javascript
function Reporter(lines, ruleset, allow, ignore) {
    "use strict";

<span class="apidocCodeCommentSpan">    /**
     * List of messages being reported.
     * @property messages
     * @type String[]
     */
</span>    this.messages = [];

    /**
     * List of statistics being reported.
     * @property stats
     * @type String[]
     */
    this.stats = [];

    /**
     * Lines of code being reported on. Used to provide contextual information
     * for messages.
     * @property lines
     * @type String[]
     */
    this.lines = lines;

    /**
     * Information about the rules. Used to determine whether an issue is an
     * error or warning.
     * @property ruleset
     * @type Object
     */
    this.ruleset = ruleset;

    /**
     * Lines with specific rule messages to leave out of the report.
     * @property allow
     * @type Object
     */
    this.allow = allow;
    if (!this.allow) {
        this.allow = {};
    }

    /**
     * Linesets not to include in the report.
     * @property ignore
     * @type [][]
     */
    this.ignore = ignore;
    if (!this.ignore) {
        this.ignore = [];
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.csslint.CSSLint"></a>[module csslint.CSSLint](#apidoc.module.csslint.CSSLint)

#### <a name="apidoc.element.csslint.CSSLint._Reporter"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint.</span>_Reporter (lines, ruleset, allow, ignore)](#apidoc.element.csslint.CSSLint._Reporter)
- description and source-code
```javascript
function Reporter(lines, ruleset, allow, ignore) {
    "use strict";

<span class="apidocCodeCommentSpan">    /**
     * List of messages being reported.
     * @property messages
     * @type String[]
     */
</span>    this.messages = [];

    /**
     * List of statistics being reported.
     * @property stats
     * @type String[]
     */
    this.stats = [];

    /**
     * Lines of code being reported on. Used to provide contextual information
     * for messages.
     * @property lines
     * @type String[]
     */
    this.lines = lines;

    /**
     * Information about the rules. Used to determine whether an issue is an
     * error or warning.
     * @property ruleset
     * @type Object
     */
    this.ruleset = ruleset;

    /**
     * Lines with specific rule messages to leave out of the report.
     * @property allow
     * @type Object
     */
    this.allow = allow;
    if (!this.allow) {
        this.allow = {};
    }

    /**
     * Linesets not to include in the report.
     * @property ignore
     * @type [][]
     */
    this.ignore = ignore;
    if (!this.ignore) {
        this.ignore = [];
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint.addFormatter"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint.</span>addFormatter (formatter)](#apidoc.element.csslint.CSSLint.addFormatter)
- description and source-code
```javascript
addFormatter = function (formatter) {
    // formatters.push(formatter);
    formatters[formatter.id] = formatter;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint.addRule"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint.</span>addRule (rule)](#apidoc.element.csslint.CSSLint.addRule)
- description and source-code
```javascript
addRule = function (rule) {
    rules.push(rule);
    rules[rule.id] = rule;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint.clearRules"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint.</span>clearRules ()](#apidoc.element.csslint.CSSLint.clearRules)
- description and source-code
```javascript
clearRules = function () {
    rules = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint.format"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint.</span>format (results, filename, formatId, options)](#apidoc.element.csslint.CSSLint.format)
- description and source-code
```javascript
format = function (results, filename, formatId, options) {
    var formatter = this.getFormatter(formatId),
        result = null;

    if (formatter) {
        result = formatter.startFormat();
        result += formatter.formatResults(results, filename, options || {});
        result += formatter.endFormat();
    }

    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint.getFormatter"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint.</span>getFormatter (formatId)](#apidoc.element.csslint.CSSLint.getFormatter)
- description and source-code
```javascript
getFormatter = function (formatId) {
    return formatters[formatId];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint.getRules"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint.</span>getRules ()](#apidoc.element.csslint.CSSLint.getRules)
- description and source-code
```javascript
getRules = function () {
    return [].concat(rules).sort(function(a, b) {
        return a.id > b.id ? 1 : 0;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint.getRuleset"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint.</span>getRuleset ()](#apidoc.element.csslint.CSSLint.getRuleset)
- description and source-code
```javascript
getRuleset = function () {
    var ruleset = {},
        i = 0,
        len = rules.length;

    while (i < len) {
        ruleset[rules[i++].id] = 1;    // by default, everything is a warning
    }

    return ruleset;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint.hasFormat"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint.</span>hasFormat (formatId)](#apidoc.element.csslint.CSSLint.hasFormat)
- description and source-code
```javascript
hasFormat = function (formatId) {
    return formatters.hasOwnProperty(formatId);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint.verify"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint.</span>verify (text, ruleset)](#apidoc.element.csslint.CSSLint.verify)
- description and source-code
```javascript
verify = function (text, ruleset) {

    var i = 0,
        reporter,
        lines,
        allow = {},
        ignore = [],
        report,
        parser = new parserlib.css.Parser({
            starHack: true,
            ieFilters: true,
            underscoreHack: true,
            strict: false
        });

    // normalize line endings
    lines = text.replace(/\n\r?/g, "$split$").split("$split$");

    // find 'allow' comments
    CSSLint.Util.forEach(lines, function (line, lineno) {
        var allowLine = line && line.match(/\/\*[ \t]*csslint[ \t]+allow:[ \t]*([^\*]*)\*\//i),
            allowRules = allowLine && allowLine[1],
            allowRuleset = {};

        if (allowRules) {
            allowRules.toLowerCase().split(",").forEach(function(allowRule) {
                allowRuleset[allowRule.trim()] = true;
            });
            if (Object.keys(allowRuleset).length > 0) {
                allow[lineno + 1] = allowRuleset;
            }
        }
    });

    var ignoreStart = null,
        ignoreEnd = null;
    CSSLint.Util.forEach(lines, function (line, lineno) {
        // Keep oldest, "unclosest" ignore:start
        if (ignoreStart === null && line.match(/\/\*[ \t]*csslint[ \t]+ignore:start[ \t]*\*\//i)) {
            ignoreStart = lineno;
        }

        if (line.match(/\/\*[ \t]*csslint[ \t]+ignore:end[ \t]*\*\//i)) {
            ignoreEnd = lineno;
        }

        if (ignoreStart !== null && ignoreEnd !== null) {
            ignore.push([ignoreStart, ignoreEnd]);
            ignoreStart = ignoreEnd = null;
        }
    });

    // Close remaining ignore block, if any
    if (ignoreStart !== null) {
        ignore.push([ignoreStart, lines.length]);
    }

    if (!ruleset) {
        ruleset = this.getRuleset();
    }

    if (embeddedRuleset.test(text)) {
        // defensively copy so that caller's version does not get modified
        ruleset = clone(ruleset);
        ruleset = applyEmbeddedRuleset(text, ruleset);
    }

    reporter = new Reporter(lines, ruleset, allow, ignore);

    ruleset.errors = 2;       // always report parsing errors as errors
    for (i in ruleset) {
        if (ruleset.hasOwnProperty(i) && ruleset[i]) {
            if (rules[i]) {
                rules[i].init(parser, reporter);
            }
        }
    }


    // capture most horrible error type
    try {
        parser.parse(text);
    } catch (ex) {
        reporter.error("Fatal error, cannot continue: " + ex.message, ex.line, ex.col, {});
    }

    report = {
        messages    : reporter.messages,
        stats       : reporter.stats,
        ruleset     : reporter.ruleset,
        allow       : reporter.allow,
        ignore      : reporter.ignore
    };

    // sort by line numbers, rollups at the bottom
    report.messages.sort(function (a, b) {
        if (a.rollup && !b.rollup) {
            return 1;
        } else if (!a.rollup && b.rollup) {
            return -1;
        } else {
            return a.line - b.line;
        }
    });

    return report;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.csslint.CSSLint.Util"></a>[module csslint.CSSLint.Util](#apidoc.module.csslint.CSSLint.Util)

#### <a name="apidoc.element.csslint.CSSLint.Util.forEach"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint.Util.</span>forEach (values, func)](#apidoc.element.csslint.CSSLint.Util.forEach)
- description and source-code
```javascript
forEach = function (values, func) {
    "use strict";
    if (values.forEach) {
        return values.forEach(func);
    } else {
        for (var i=0, len=values.length; i < len; i++) {
            func(values[i], i, values);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint.Util.indexOf"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint.Util.</span>indexOf (values, value)](#apidoc.element.csslint.CSSLint.Util.indexOf)
- description and source-code
```javascript
indexOf = function (values, value) {
    "use strict";
    if (values.indexOf) {
        return values.indexOf(value);
    } else {
        for (var i=0, len=values.length; i < len; i++) {
            if (values[i] === value) {
                return i;
            }
        }
        return -1;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint.Util.mix"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint.Util.</span>mix (receiver, supplier)](#apidoc.element.csslint.CSSLint.Util.mix)
- description and source-code
```javascript
mix = function (receiver, supplier) {
    "use strict";
    var prop;

    for (prop in supplier) {
        if (supplier.hasOwnProperty(prop)) {
            receiver[prop] = supplier[prop];
        }
    }

    return prop;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.csslint.CSSLint._Reporter"></a>[module csslint.CSSLint._Reporter](#apidoc.module.csslint.CSSLint._Reporter)

#### <a name="apidoc.element.csslint.CSSLint._Reporter._Reporter"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint.</span>_Reporter (lines, ruleset, allow, ignore)](#apidoc.element.csslint.CSSLint._Reporter._Reporter)
- description and source-code
```javascript
function Reporter(lines, ruleset, allow, ignore) {
    "use strict";

<span class="apidocCodeCommentSpan">    /**
     * List of messages being reported.
     * @property messages
     * @type String[]
     */
</span>    this.messages = [];

    /**
     * List of statistics being reported.
     * @property stats
     * @type String[]
     */
    this.stats = [];

    /**
     * Lines of code being reported on. Used to provide contextual information
     * for messages.
     * @property lines
     * @type String[]
     */
    this.lines = lines;

    /**
     * Information about the rules. Used to determine whether an issue is an
     * error or warning.
     * @property ruleset
     * @type Object
     */
    this.ruleset = ruleset;

    /**
     * Lines with specific rule messages to leave out of the report.
     * @property allow
     * @type Object
     */
    this.allow = allow;
    if (!this.allow) {
        this.allow = {};
    }

    /**
     * Linesets not to include in the report.
     * @property ignore
     * @type [][]
     */
    this.ignore = ignore;
    if (!this.ignore) {
        this.ignore = [];
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.csslint.CSSLint._Reporter.prototype"></a>[module csslint.CSSLint._Reporter.prototype](#apidoc.module.csslint.CSSLint._Reporter.prototype)

#### <a name="apidoc.element.csslint.CSSLint._Reporter.prototype.constructor"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint._Reporter.prototype.</span>constructor (lines, ruleset, allow, ignore)](#apidoc.element.csslint.CSSLint._Reporter.prototype.constructor)
- description and source-code
```javascript
function Reporter(lines, ruleset, allow, ignore) {
    "use strict";

<span class="apidocCodeCommentSpan">    /**
     * List of messages being reported.
     * @property messages
     * @type String[]
     */
</span>    this.messages = [];

    /**
     * List of statistics being reported.
     * @property stats
     * @type String[]
     */
    this.stats = [];

    /**
     * Lines of code being reported on. Used to provide contextual information
     * for messages.
     * @property lines
     * @type String[]
     */
    this.lines = lines;

    /**
     * Information about the rules. Used to determine whether an issue is an
     * error or warning.
     * @property ruleset
     * @type Object
     */
    this.ruleset = ruleset;

    /**
     * Lines with specific rule messages to leave out of the report.
     * @property allow
     * @type Object
     */
    this.allow = allow;
    if (!this.allow) {
        this.allow = {};
    }

    /**
     * Linesets not to include in the report.
     * @property ignore
     * @type [][]
     */
    this.ignore = ignore;
    if (!this.ignore) {
        this.ignore = [];
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint._Reporter.prototype.error"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint._Reporter.prototype.</span>error (message, line, col, rule)](#apidoc.element.csslint.CSSLint._Reporter.prototype.error)
- description and source-code
```javascript
error = function (message, line, col, rule) {
    "use strict";
    this.messages.push({
        type    : "error",
        line    : line,
        col     : col,
        message : message,
        evidence: this.lines[line-1],
        rule    : rule || {}
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint._Reporter.prototype.info"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint._Reporter.prototype.</span>info (message, line, col, rule)](#apidoc.element.csslint.CSSLint._Reporter.prototype.info)
- description and source-code
```javascript
info = function (message, line, col, rule) {
    "use strict";
    this.messages.push({
        type    : "info",
        line    : line,
        col     : col,
        message : message,
        evidence: this.lines[line-1],
        rule    : rule
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint._Reporter.prototype.report"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint._Reporter.prototype.</span>report (message, line, col, rule)](#apidoc.element.csslint.CSSLint._Reporter.prototype.report)
- description and source-code
```javascript
report = function (message, line, col, rule) {
    "use strict";

    // Check if rule violation should be allowed
    if (this.allow.hasOwnProperty(line) && this.allow[line].hasOwnProperty(rule.id)) {
        return;
    }

    var ignore = false;
    CSSLint.Util.forEach(this.ignore, function (range) {
        if (range[0] <= line && line <= range[1]) {
            ignore = true;
        }
    });
    if (ignore) {
        return;
    }

    this.messages.push({
        type    : this.ruleset[rule.id] === 2 ? "error" : "warning",
        line    : line,
        col     : col,
        message : message,
        evidence: this.lines[line-1],
        rule    : rule
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint._Reporter.prototype.rollupError"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint._Reporter.prototype.</span>rollupError (message, rule)](#apidoc.element.csslint.CSSLint._Reporter.prototype.rollupError)
- description and source-code
```javascript
rollupError = function (message, rule) {
    "use strict";
    this.messages.push({
        type    : "error",
        rollup  : true,
        message : message,
        rule    : rule
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint._Reporter.prototype.rollupWarn"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint._Reporter.prototype.</span>rollupWarn (message, rule)](#apidoc.element.csslint.CSSLint._Reporter.prototype.rollupWarn)
- description and source-code
```javascript
rollupWarn = function (message, rule) {
    "use strict";
    this.messages.push({
        type    : "warning",
        rollup  : true,
        message : message,
        rule    : rule
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint._Reporter.prototype.stat"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint._Reporter.prototype.</span>stat (name, value)](#apidoc.element.csslint.CSSLint._Reporter.prototype.stat)
- description and source-code
```javascript
stat = function (name, value) {
    "use strict";
    this.stats[name] = value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.csslint.CSSLint._Reporter.prototype.warn"></a>[function <span class="apidocSignatureSpan">csslint.CSSLint._Reporter.prototype.</span>warn (message, line, col, rule)](#apidoc.element.csslint.CSSLint._Reporter.prototype.warn)
- description and source-code
```javascript
warn = function (message, line, col, rule) {
    "use strict";
    this.report(message, line, col, rule);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
