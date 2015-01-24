Generous JSON
=============

Generous JSON is a JSON parser that supports comments and unquoted strings.
You know, for people.

It is a combination of:
 * [JSOL](https://github.com/daepark/JSOL) by Dae Park
 * [JSON.minify](https://github.com/getify/JSON.minify) by Kyle Simpson

Example of a Generous JSON document
-----------------------------------

    {
        unquotedStrings: "are ok",

        // Single line comments are too.
        "cat": true,

        /*
         * And multi-line comments
         */
        riesling: "schloss vollrads"
    }

API
---

### GenerousJSON.parse(&lt;String&gt; jsonString) ###
Generously parses a JSON document.

Returns the parsed object.
Throws an error if the JSON string is invalid.
