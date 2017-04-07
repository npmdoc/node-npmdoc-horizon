# api documentation for  [horizon (v2.0.0)](https://github.com/rethinkdb/horizon#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-horizon.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-horizon) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-horizon.svg)](https://travis-ci.org/npmdoc/node-npmdoc-horizon)
#### An open-source developer platform for building realtime, scalable web apps.

[![NPM](https://nodei.co/npm/horizon.png?downloads=true)](https://www.npmjs.com/package/horizon)

[![apidoc](https://npmdoc.github.io/node-npmdoc-horizon/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-horizon_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-horizon/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-horizon/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-horizon/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "RethinkDB"
    },
    "bin": {
        "hz": "src/main.js",
        "horizon": "src/main.js"
    },
    "bugs": {
        "url": "https://github.com/rethinkdb/horizon/issues"
    },
    "dependencies": {
        "@horizon/server": "2.0.0",
        "argparse": "^1.0.3",
        "bluebird": "^3.4.1",
        "chalk": "^1.1.3",
        "hasbin": "^1.2.1",
        "joi": "^8.0.5",
        "jsonwebtoken": "^5.5.4",
        "mime-types": "^2.0.4",
        "open": "0.0.5",
        "rethinkdb": "^2.1.1",
        "toml": "^2.3.0"
    },
    "description": "An open-source developer platform for building realtime, scalable web apps.",
    "devDependencies": {
        "chai": "^3.5.0",
        "eslint": "^2.3.0",
        "istanbul": "^0.4.3",
        "mocha": "2.4.5",
        "mock-fs": "^3.10.0",
        "sinon": "1.17.3",
        "strip-ansi": "^3.0.1",
        "toml": "^2.3.0"
    },
    "directories": {},
    "dist": {
        "shasum": "0049b36faeae7779f048d7cc07d0b77b4ca9c3d7",
        "tarball": "https://registry.npmjs.org/horizon/-/horizon-2.0.0.tgz"
    },
    "engines": {
        "node": ">=4.0.0",
        "npm": ">=3.0.0"
    },
    "homepage": "https://github.com/rethinkdb/horizon#readme",
    "license": "MIT",
    "main": "src/main.js",
    "maintainers": [
        {
            "name": "rethinkdb",
            "email": "bugs@rethinkdb.com"
        }
    ],
    "name": "horizon",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/rethinkdb/horizon.git"
    },
    "scripts": {
        "coverage": "istanbul cover _mocha test",
        "lint": "eslint src test",
        "test": "mocha test test/unit --timeout 10000"
    },
    "version": "2.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module horizon](#apidoc.module.horizon)
1.  object <span class="apidocSignatureSpan">horizon.</span>create_cert
1.  object <span class="apidocSignatureSpan">horizon.</span>init
1.  object <span class="apidocSignatureSpan">horizon.</span>make_token
1.  object <span class="apidocSignatureSpan">horizon.</span>migrate
1.  object <span class="apidocSignatureSpan">horizon.</span>schema
1.  object <span class="apidocSignatureSpan">horizon.</span>serve
1.  object <span class="apidocSignatureSpan">horizon.</span>version

#### [module horizon.create_cert](#apidoc.module.horizon.create_cert)
1.  [function <span class="apidocSignatureSpan">horizon.create_cert.</span>run (args)](#apidoc.element.horizon.create_cert.run)
1.  string <span class="apidocSignatureSpan">horizon.create_cert.</span>description

#### [module horizon.init](#apidoc.module.horizon.init)
1.  [function <span class="apidocSignatureSpan">horizon.init.</span>run (args)](#apidoc.element.horizon.init.run)
1.  string <span class="apidocSignatureSpan">horizon.init.</span>description

#### [module horizon.make_token](#apidoc.module.horizon.make_token)
1.  [function <span class="apidocSignatureSpan">horizon.make_token.</span>run (args)](#apidoc.element.horizon.make_token.run)
1.  string <span class="apidocSignatureSpan">horizon.make_token.</span>description

#### [module horizon.migrate](#apidoc.module.horizon.migrate)
1.  [function <span class="apidocSignatureSpan">horizon.migrate.</span>run (cmdArgs)](#apidoc.element.horizon.migrate.run)
1.  string <span class="apidocSignatureSpan">horizon.migrate.</span>description

#### [module horizon.schema](#apidoc.module.horizon.schema)
1.  [function <span class="apidocSignatureSpan">horizon.schema.</span>parse_schema (schema_toml)](#apidoc.element.horizon.schema.parse_schema)
1.  [function <span class="apidocSignatureSpan">horizon.schema.</span>processApplyConfig (parsed)](#apidoc.element.horizon.schema.processApplyConfig)
1.  [function <span class="apidocSignatureSpan">horizon.schema.</span>run (args)](#apidoc.element.horizon.schema.run)
1.  [function <span class="apidocSignatureSpan">horizon.schema.</span>runApplyCommand (options)](#apidoc.element.horizon.schema.runApplyCommand)
1.  [function <span class="apidocSignatureSpan">horizon.schema.</span>runSaveCommand (options)](#apidoc.element.horizon.schema.runSaveCommand)
1.  string <span class="apidocSignatureSpan">horizon.schema.</span>description

#### [module horizon.serve](#apidoc.module.horizon.serve)
1.  [function <span class="apidocSignatureSpan">horizon.serve.</span>parseArguments (args)](#apidoc.element.horizon.serve.parseArguments)
1.  [function <span class="apidocSignatureSpan">horizon.serve.</span>processConfig (parsed)](#apidoc.element.horizon.serve.processConfig)
1.  [function <span class="apidocSignatureSpan">horizon.serve.</span>run (args, interruptor)](#apidoc.element.horizon.serve.run)
1.  string <span class="apidocSignatureSpan">horizon.serve.</span>description

#### [module horizon.version](#apidoc.module.horizon.version)
1.  [function <span class="apidocSignatureSpan">horizon.version.</span>run (args)](#apidoc.element.horizon.version.run)
1.  string <span class="apidocSignatureSpan">horizon.version.</span>description



# <a name="apidoc.module.horizon"></a>[module horizon](#apidoc.module.horizon)



# <a name="apidoc.module.horizon.create_cert"></a>[module horizon.create_cert](#apidoc.module.horizon.create_cert)

#### <a name="apidoc.element.horizon.create_cert.run"></a>[function <span class="apidocSignatureSpan">horizon.create_cert.</span>run (args)](#apidoc.element.horizon.create_cert.run)
- description and source-code
```javascript
(args) => {
  if (args.length) {
    throw new Error('create-cert takes no arguments');
  }

  // TODO: user configuration?
  const settings = {
    binaryName: 'openssl',
    keyOutName: 'horizon-key.pem',
    certOutName: 'horizon-cert.pem',
    algo: 'rsa',
    bits: '2048',
    days: '365',
  };

  // generate the arguments to the command
  const binArgs = [ 'req', '-x509', '-nodes', '-batch',
    '-newkey', '${settings.algo}:${settings.bits}',
    '-keyout', settings.keyOutName,
    '-out', settings.certOutName,
    '-days', settings.days,
  ];

  return new Promise((resolve, reject) => {
    hasbin(settings.binaryName, (hasOpenSSL) => {
      // show the invocation that's about to be run
      console.log('> ${settings.binaryName} ${binArgs.join(' ')}');

      // if we don't have openssl, bail
      if (!hasOpenSSL) {
        reject(new Error('Missing ${settings.binaryName}. Make sure it is on the path.'));
      }

      // otherwise start openssl
      const sslProc = spawn(settings.binaryName, binArgs);

      // pipe output appropriately
      sslProc.stdout.pipe(process.stdout, { end: false });
      sslProc.stderr.pipe(process.stderr, { end: false });

      // say nice things to the user when it's done
      sslProc.on('error', reject);
      sslProc.on('close', (code) => {
        if (code) {
          reject(new Error('OpenSSL failed with code ${code}.'));
        } else {
          console.log('Everything seems to be fine. ' +
                      'Remember to add your shiny new certificates to your Horizon config!');
          resolve();
        }
      });
    });
  });
}
```
- example usage
```shell
...

  return Promise.resolve().then(() => {
    white('Validating current schema version');
    return r.dbList().contains('${project}_internal')
      .branch(true, r.error(internalNotFound))
      .do(() => checkForHzTables)
      .do(() => waitForCollections)
      .run(this.conn)
      .then(() => green(' └── Pre-2.0 schema found'))
      .catch((e) => {
        if (e.msg === internalNotFound) {
          throw new NiceError(e.msg, {
            description: '\
This could happen if you don't have a Horizon app in this database, or if \
you've already migrated this database to the v2.0 format.',
...
```



# <a name="apidoc.module.horizon.init"></a>[module horizon.init](#apidoc.module.horizon.init)

#### <a name="apidoc.element.horizon.init.run"></a>[function <span class="apidocSignatureSpan">horizon.init.</span>run (args)](#apidoc.element.horizon.init.run)
- description and source-code
```javascript
(args) =>
  Promise.resolve(args)
.then(parseArguments)
.then((parsed) => {
  const check = checkProjectName(
    parsed.projectName,
    process.cwd(),
    fs.readdirSync('.')
  );
  const projectName = check.projectName;
  const dirName = check.dirName;
  const chdirTo = check.chdirTo;
  const createDir = check.createDir;
  maybeMakeDir(createDir, dirName);
  maybeChdir(chdirTo);

  // Before we create things, check if the directory is empty
  const dirWasPopulated = fs.readdirSync(process.cwd()).length !== 0;
  populateDir(projectName, dirWasPopulated, chdirTo, dirName);
})
```
- example usage
```shell
...

  return Promise.resolve().then(() => {
    white('Validating current schema version');
    return r.dbList().contains('${project}_internal')
      .branch(true, r.error(internalNotFound))
      .do(() => checkForHzTables)
      .do(() => waitForCollections)
      .run(this.conn)
      .then(() => green(' └── Pre-2.0 schema found'))
      .catch((e) => {
        if (e.msg === internalNotFound) {
          throw new NiceError(e.msg, {
            description: '\
This could happen if you don't have a Horizon app in this database, or if \
you've already migrated this database to the v2.0 format.',
...
```



# <a name="apidoc.module.horizon.make_token"></a>[module horizon.make_token](#apidoc.module.horizon.make_token)

#### <a name="apidoc.element.horizon.make_token.run"></a>[function <span class="apidocSignatureSpan">horizon.make_token.</span>run (args)](#apidoc.element.horizon.make_token.run)
- description and source-code
```javascript
(args) => Promise.resolve().then(() => {
  const options = processConfig(parseArguments(args));

  if (options.token_secret === null) {
    throw new Error('No token secret specified, unable to sign the token.');
  }
  const token = jwt.sign(
    { id: options.user, provider: null },
    new Buffer(options.token_secret, 'base64'),
    { expiresIn: '1d', algorithm: 'HS512' }
  );
  console.log('${token}');
})
```
- example usage
```shell
...

  return Promise.resolve().then(() => {
    white('Validating current schema version');
    return r.dbList().contains('${project}_internal')
      .branch(true, r.error(internalNotFound))
      .do(() => checkForHzTables)
      .do(() => waitForCollections)
      .run(this.conn)
      .then(() => green(' └── Pre-2.0 schema found'))
      .catch((e) => {
        if (e.msg === internalNotFound) {
          throw new NiceError(e.msg, {
            description: '\
This could happen if you don't have a Horizon app in this database, or if \
you've already migrated this database to the v2.0 format.',
...
```



# <a name="apidoc.module.horizon.migrate"></a>[module horizon.migrate](#apidoc.module.horizon.migrate)

#### <a name="apidoc.element.horizon.migrate.run"></a>[function <span class="apidocSignatureSpan">horizon.migrate.</span>run (cmdArgs)](#apidoc.element.horizon.migrate.run)
- description and source-code
```javascript
function run(cmdArgs) {
  const options = processConfig(cmdArgs);
  interrupt.on_interrupt(() => teardown());
  return Promise.resolve().bind({ options })
    .then(setup)
    .then(validateMigration)
    .then(makeBackup)
    .then(renameUserTables)
    .then(moveInternalTables)
    .then(renameIndices)
    .then(rewriteHzCollectionDocs)
    .then(exportNewSchema)
    .finally(teardown);
}
```
- example usage
```shell
...

  return Promise.resolve().then(() => {
    white('Validating current schema version');
    return r.dbList().contains('${project}_internal')
      .branch(true, r.error(internalNotFound))
      .do(() => checkForHzTables)
      .do(() => waitForCollections)
      .run(this.conn)
      .then(() => green(' └── Pre-2.0 schema found'))
      .catch((e) => {
        if (e.msg === internalNotFound) {
          throw new NiceError(e.msg, {
            description: '\
This could happen if you don't have a Horizon app in this database, or if \
you've already migrated this database to the v2.0 format.',
...
```



# <a name="apidoc.module.horizon.schema"></a>[module horizon.schema](#apidoc.module.horizon.schema)

#### <a name="apidoc.element.horizon.schema.parse_schema"></a>[function <span class="apidocSignatureSpan">horizon.schema.</span>parse_schema (schema_toml)](#apidoc.element.horizon.schema.parse_schema)
- description and source-code
```javascript
(schema_toml) => {
  const parsed = Joi.validate(toml.parse(schema_toml), schema_schema);
  const schema = parsed.value;

  if (parsed.error) {
    throw parsed.error;
  }

  const collections = [ ];
  for (const name in schema.collections) {
    collections.push({
      id: name,
      indexes: schema.collections[name].indexes.map((index) => {
        if (typeof index === 'string') {
          return { fields: v1_0_name_to_fields(index), multi: false, geo: false };
        } else {
          return { fields: index.fields, multi: false, geo: false };
        }
      }),
    });
  }

  // Make sure the 'users' collection is present, as some things depend on
  // its existence.
  if (!schema.collections || !schema.collections.users) {
    collections.push({ id: 'users', indexes: [ ] });
  }

  const groups = [ ];
  for (const name in schema.groups) {
    groups.push(Object.assign({ id: name }, schema.groups[name]));
  }

  return { groups, collections };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.horizon.schema.processApplyConfig"></a>[function <span class="apidocSignatureSpan">horizon.schema.</span>processApplyConfig (parsed)](#apidoc.element.horizon.schema.processApplyConfig)
- description and source-code
```javascript
(parsed) => {
  let options, in_file;

  options = config.default_options();
  options = config.merge_options(options,
    config.read_from_config_file(parsed.project_path));
  options = config.merge_options(options, config.read_from_env());
  options = config.merge_options(options, config.read_from_flags(parsed));

  if (parsed.schema_file === '-') {
    in_file = process.stdin;
  } else {
    in_file = fs.createReadStream(parsed.schema_file, { flags: 'r' });
  }

  if (options.project_name === null) {
    options.project_name = path.basename(path.resolve(options.project_path));
  }

  return {
    subcommand_name: 'apply',
    start_rethinkdb: options.start_rethinkdb,
    rdb_host: options.rdb_host,
    rdb_port: options.rdb_port,
    project_name: options.project_name,
    project_path: options.project_path,
    debug: options.debug,
    update: parse_yes_no_option(parsed.update),
    force: parse_yes_no_option(parsed.force),
    in_file,
  };
}
```
- example usage
```shell
...
try {
  fs.accessAsync(opts.schema_file, fs.R_OK | fs.F_OK);
} catch (e) {
  console.error(
    chalk.yellow.bold('No .hz/schema.toml file found'));
  return;
}
const schemaOptions = schema.processApplyConfig({
  project_name: opts.project_name,
  schema_file: opts.schema_file,
  start_rethinkdb: false,
  connect: '${opts.rdb_host}:${opts.rdb_port}',
  update: true,
  force: false,
});
...
```

#### <a name="apidoc.element.horizon.schema.run"></a>[function <span class="apidocSignatureSpan">horizon.schema.</span>run (args)](#apidoc.element.horizon.schema.run)
- description and source-code
```javascript
(args) =>
Promise.resolve().then(() => {
  const options = processConfig(parseArguments(args));
  // Determine if we are saving or applying and use appropriate run function
  switch (options.subcommand_name) {
  case 'apply':
    return runApplyCommand(options);
  case 'save':
    return runSaveCommand(options);
  default:
    throw new Error('Unrecognized schema subcommand: "${options.subcommand_name}"');
  }
})
```
- example usage
```shell
...

  return Promise.resolve().then(() => {
    white('Validating current schema version');
    return r.dbList().contains('${project}_internal')
      .branch(true, r.error(internalNotFound))
      .do(() => checkForHzTables)
      .do(() => waitForCollections)
      .run(this.conn)
      .then(() => green(' └── Pre-2.0 schema found'))
      .catch((e) => {
        if (e.msg === internalNotFound) {
          throw new NiceError(e.msg, {
            description: '\
This could happen if you don't have a Horizon app in this database, or if \
you've already migrated this database to the v2.0 format.',
...
```

#### <a name="apidoc.element.horizon.schema.runApplyCommand"></a>[function <span class="apidocSignatureSpan">horizon.schema.</span>runApplyCommand (options)](#apidoc.element.horizon.schema.runApplyCommand)
- description and source-code
```javascript
(options) => {
  let conn, schema, rdb_server;
  let obsolete_collections = [ ];
  const db = options.project_name;

  const cleanup = () =>
    Promise.all([
      conn ? conn.close() : Promise.resolve(),
      rdb_server ? rdb_server.close() : Promise.resolve(),
    ]);

  interrupt.on_interrupt(() => cleanup());

  return Promise.resolve().then(() => {
    if (options.start_rethinkdb) {
      change_to_project_dir(options.project_path);
    }

    return new Promise((resolve, reject) => {
      let schema_toml = '';
      options.in_file.on('data', (buffer) => (schema_toml += buffer));
      options.in_file.on('end', () => resolve(schema_toml));
      options.in_file.on('error', reject);
    });
  }).then((schema_toml) => {
    schema = parse_schema(schema_toml);

    if (options.start_rethinkdb) {
      return start_rdb_server({ quiet: !options.debug }).then((server) => {
        rdb_server = server;
        options.rdb_host = 'localhost';
        options.rdb_port = server.driver_port;
      });
    }
  }).then(() =>
    r.connect({ host: options.rdb_host,
                port: options.rdb_port,
                user: options.rdb_user,
                password: options.rdb_password,
                timeout: options.rdb_timeout })
  ).then((rdb_conn) => {
    conn = rdb_conn;
    return initialize_metadata(db, conn);
  }).then((initialization_result) => {
    if (initialization_result.tables_created) {
      console.log('Initialized new application metadata.');
    }
    // Wait for metadata tables to be writable
    return r.expr([ 'hz_collections', 'hz_groups' ])
      .forEach((table) =>
        r.db(db).table(table)
          .wait({ waitFor: 'ready_for_writes', timeout: 30 }))
      .run(conn);
  }).then(() => {
    // Error if any collections will be removed
    if (!options.update) {
      return r.db(db).table('hz_collections')
        .filter((row) => row('id').match('^hz_').not())
        .getField('id')
        .coerceTo('array')
        .setDifference(schema.collections.map((c) => c.id))
        .run(conn)
        .then((res) => {
          if (!options.force && res.length > 0) {
            throw new Error('Run with "--force" to continue.\n' +
                            'These collections would be removed along with their data:\n' +
                            '${res.join(', ')}');
          }
          obsolete_collections = res;
        });
    }
  }).then(() => {
    if (options.update) {
      // Update groups
      return Promise.all(schema.groups.map((group) => {
        const literal_group = JSON.parse(JSON.stringify(group));
        Object.keys(literal_group.rules).forEach((key) => {
          literal_group.rules[key] = r.literal(literal_group.rules[key]);
        });

        return r.db(db).table('hz_groups')
          .get(group.id).replace((old_row) =>
            r.branch(old_row.eq(null),
                     group,
                     old_row.merge(literal_group)))
          .run(conn).then((res) => {
            if (res.errors) {
              throw new Error('Failed to update group: ${res.first_error}');
            }
          });
      }));
    } else {
      // Replace and remove groups
      const groups_obj = { };
      schema.groups.forEach((g) => { groups_obj[g.id] = g; });

      return Promise.all([
        r.expr(groups_obj).do((groups) =>
          r.db(db).table('hz_groups')
            .replace((old_row) =>
              r.branch(groups.hasFields(old_row('id')),
                       old_row,
                       null))
          ).run(conn).then((res) => {
            if (res.errors) {
              throw new Error('Failed to write groups: ${res.first_error}');
            }
          }),
        r.db(db).table('hz_groups')
          .insert(schema.groups, { conflict: 'replace' })
          .run(conn).then((res) => {
            if (res.errors) {
              throw new Error('Failed to write groups: ${res.first_error}');
            }
          }),
      ]);
    }
  }).then(() => {
    // Ensure all collections exist and remove any obsolete collections
    const promise ...
```
- example usage
```shell
...
    project_name: opts.project_name,
    schema_file: opts.schema_file,
    start_rethinkdb: false,
    connect: '${opts.rdb_host}:${opts.rdb_port}',
    update: true,
    force: false,
  });
  return schema.runApplyCommand(schemaOptions);
}
  }).then(() => {
console.log('Starting Horizon...');
hz_server = start_horizon_server(http_servers, opts);

return new Promise((resolve, reject) => {
  const timeoutObject = setTimeout(() => {
...
```

#### <a name="apidoc.element.horizon.schema.runSaveCommand"></a>[function <span class="apidocSignatureSpan">horizon.schema.</span>runSaveCommand (options)](#apidoc.element.horizon.schema.runSaveCommand)
- description and source-code
```javascript
(options) => {
  let conn, rdb_server;
  const db = options.project_name;

  const cleanup = () =>
    Promise.all([
      conn ? conn.close() : Promise.resolve(),
      rdb_server ? rdb_server.close() : Promise.resolve(),
    ]);

  interrupt.on_interrupt(() => cleanup());

  return Promise.resolve().then(() => {
    if (options.start_rethinkdb) {
      change_to_project_dir(options.project_path);
    }
  }).then(() => {
    if (options.start_rethinkdb) {
      return start_rdb_server({ quiet: !options.debug }).then((server) => {
        rdb_server = server;
        options.rdb_host = 'localhost';
        options.rdb_port = server.driver_port;
      });
    }
  }).then(() =>
    r.connect({ host: options.rdb_host,
                port: options.rdb_port,
                user: options.rdb_user,
                password: options.rdb_password,
                timeout: options.rdb_timeout })
  ).then((rdb_conn) => {
    conn = rdb_conn;
    return r.db(db).wait({ waitFor: 'ready_for_reads', timeout: 30 }).run(conn);
  }).then(() =>
    r.object('collections',
             r.db(db).table('hz_collections')
               .filter((row) => row('id').match('^hz_').not())
               .coerceTo('array')
               .map((row) =>
                 row.merge({ indexes: r.db(db).table(row('id')).indexList() })),
             'groups', r.db(db).table('hz_groups').coerceTo('array'))
      .run(conn)
  ).then((res) =>
    new Promise((resolve) => {
      // Only rename old file if saving to default .hz/schema.toml
      if (options.out_file === '.hz/schema.toml' &&
          file_exists(options.out_file)) {
        // Rename existing file to have the current time appended to its name
        const oldPath = path.resolve(options.out_file);
        const newPath = '${path.resolve(options.out_file)}.${new Date().toISOString()}';
        fs.renameSync(oldPath, newPath);
      }

      const output = (options.out_file === '-') ? process.stdout :
        fs.createWriteStream(options.out_file, { flags: 'w', defaultEncoding: 'utf8' });

      // Output toml_str to schema.toml
      const toml_str = schema_to_toml(res.collections, res.groups);
      output.end(toml_str, resolve);
    })
  ).then(cleanup).catch((err) => cleanup().then(() => { throw err; }));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.horizon.serve"></a>[module horizon.serve](#apidoc.module.horizon.serve)

#### <a name="apidoc.element.horizon.serve.parseArguments"></a>[function <span class="apidocSignatureSpan">horizon.serve.</span>parseArguments (args)](#apidoc.element.horizon.serve.parseArguments)
- description and source-code
```javascript
(args) => {
  const parser = new argparse.ArgumentParser({ prog: 'hz serve' });

  parser.addArgument([ 'project_path' ],
    { type: 'string', nargs: '?',
      help: 'Change to this directory before serving' });

  parser.addArgument([ '--project-name', '-n' ],
    { type: 'string', action: 'store', metavar: 'NAME',
      help: 'Name of the Horizon project. Determines the name of ' +
            'the RethinkDB database that stores the project data.' });

  parser.addArgument([ '--bind', '-b' ],
    { type: 'string', action: 'append', metavar: 'HOST',
      help: 'Local hostname to serve horizon on (repeatable).' });

  parser.addArgument([ '--port', '-p' ],
    { type: 'int', metavar: 'PORT',
      help: 'Local port to serve horizon on.' });

  parser.addArgument([ '--connect', '-c' ],
    { type: 'string', metavar: 'HOST:PORT',
      help: 'Host and port of the RethinkDB server to connect to.' });

  parser.addArgument([ '--rdb-timeout' ],
    { type: 'int', metavar: 'TIMEOUT',
      help: 'Timeout period in seconds for the RethinkDB connection to be opened' });

  parser.addArgument([ '--rdb-user' ],
    { type: 'string', metavar: 'USER',
      help: 'RethinkDB User' });

  parser.addArgument([ '--rdb-password' ],
    { type: 'string', metavar: 'PASSWORD',
      help: 'RethinkDB Password' });

  parser.addArgument([ '--key-file' ],
    { type: 'string', metavar: 'PATH',
      help: 'Path to the key file to use, defaults to "./horizon-key.pem".' });

  parser.addArgument([ '--cert-file' ],
    { type: 'string', metavar: 'PATH',
      help: 'Path to the cert file to use, defaults to "./horizon-cert.pem".' });

  parser.addArgument([ '--token-secret' ],
    { type: 'string', metavar: 'SECRET',
      help: 'Key for signing jwts' });

  parser.addArgument([ '--allow-unauthenticated' ],
    { type: 'string', metavar: 'yes|no', constant: 'yes', nargs: '?',
      help: 'Whether to allow unauthenticated Horizon connections.' });

  parser.addArgument([ '--allow-anonymous' ],
    { type: 'string', metavar: 'yes|no', constant: 'yes', nargs: '?',
      help: 'Whether to allow anonymous Horizon connections.' });

  parser.addArgument([ '--debug' ],
    { type: 'string', metavar: 'yes|no', constant: 'yes', nargs: '?',
      help: 'Enable debug logging.' });

  parser.addArgument([ '--secure' ],
    { type: 'string', metavar: 'yes|no', constant: 'yes', nargs: '?',
      help: 'Serve secure websockets, requires --key-file and ' +
      '--cert-file if true, on by default.' });

  parser.addArgument([ '--start-rethinkdb' ],
    { type: 'string', metavar: 'yes|no', constant: 'yes', nargs: '?',
      help: 'Start up a RethinkDB server in the current directory' });

  parser.addArgument([ '--auto-create-collection' ],
    { type: 'string', metavar: 'yes|no', constant: 'yes', nargs: '?',
      help: 'Create collections used by requests if they do not exist.' });

  parser.addArgument([ '--auto-create-index' ],
    { type: 'string', metavar: 'yes|no', constant: 'yes', nargs: '?',
      help: 'Create indexes used by requests if they do not exist.' });

  parser.addArgument([ '--permissions' ],
    { type: 'string', metavar: 'yes|no', constant: 'yes', nargs: '?',
      help: 'Enables or disables checking permissions on requests.' });

  parser.addArgument([ '--serve-static' ],
    { type: 'string', metavar: 'PATH', nargs: '?', constant: './dist',
      help: 'Serve static files from a directory, defaults to "./dist".' });

  parser.addArgument([ '--dev' ],
    { action: 'storeTrue',
      help: 'Runs the server in development mode, this sets ' +
      '--secure=no, ' +
      '--permissions=no, ' +
      '--auto-create-collection=yes, ' +
      '--auto-create-index=yes, ' +
      '--start-rethinkdb=yes, ' +
      '--allow-unauthenticated=yes, ' +
      '--allow-anonymous=yes ' +
      'and --serve-static=./dist.' });

  parser.addArgument([ '--schema-file' ],
    { type: 'string', metavar: 'SCHEMA_FILE_PATH',
      help: 'Path to the schema file to use, ' +
      'will attempt to apply schema before starting Horizon server".' });

  parser.a ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.horizon.serve.processConfig"></a>[function <span class="apidocSignatureSpan">horizon.serve.</span>processConfig (parsed)](#apidoc.element.horizon.serve.processConfig)
- description and source-code
```javascript
(parsed) => {
  let options;

  options = config.default_options();

  options = config.merge_options(options,
    config.read_from_config_file(parsed.project_path));

  options = config.merge_options(options,
    config.read_from_secrets_file(parsed.project_path));

  options = config.merge_options(options, config.read_from_env());

  options = config.merge_options(options, config.read_from_flags(parsed));

  if (options.project_name === null) {
    options.project_name = path.basename(path.resolve(options.project_path));
  }

  if (options.bind.indexOf('all') !== -1) {
    options.bind = [ '0.0.0.0' ];
  }

  if (!options.rdb_host) {
    options.rdb_host = default_rdb_host;
  }

  if (!options.rdb_port) {
    options.rdb_port = default_rdb_port;
  }

  if (!options.rdb_timeout) {
    options.rdb_timeout = default_rdb_timeout;
  }

  return options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.horizon.serve.run"></a>[function <span class="apidocSignatureSpan">horizon.serve.</span>run (args, interruptor)](#apidoc.element.horizon.serve.run)
- description and source-code
```javascript
(args, interruptor) => {
  let opts, http_servers, hz_server, rdb_server;
  const old_log_level = logger.level;

  const cleanup = () => {
    logger.level = old_log_level;

    return Promise.all([
      hz_server ? hz_server.close() : Promise.resolve(),
      rdb_server ? rdb_server.close() : Promise.resolve(),
      http_servers ? Promise.all(http_servers.map((s) =>
        new Promise((resolve) => s.close(resolve)))) : Promise.resolve(),
    ]);
  };

  interrupt.on_interrupt(() => cleanup());

  return Promise.resolve().then(() => {
    opts = processConfig(parseArguments(args));
    logger.level = opts.debug ? 'debug' : 'warn';

    if (!opts.secure && opts.auth && Array.from(Object.keys(opts.auth)).length > 0) {
      logger.warn('Authentication requires that the server be accessible via HTTPS. ' +
                  'Either specify "secure=true" or use a reverse proxy.');
    }

    change_to_project_dir(opts.project_path);

    if (opts.secure) {
      return create_secure_servers(opts);
    } else {
      return create_insecure_servers(opts);
    }
  }).then((servers) => {
    http_servers = servers;

    if (opts.start_rethinkdb) {
      return start_rdb_server().then((server) => {
        rdb_server = server;

        // Don't need to check for host, always localhost.
        opts.rdb_host = 'localhost';
        opts.rdb_port = server.driver_port;

        console.log('RethinkDB');
        console.log('   ├── Admin interface: http://localhost:${server.http_port}');
        console.log('   └── Drivers can connect to port ${server.driver_port}');
      });
    }
  }).then(() => {
    // Ensure schema from schema.toml file is set
    if (opts.schema_file) {
      console.log('Ensuring schema "${opts.schema_file}" is applied');
      try {
        fs.accessAsync(opts.schema_file, fs.R_OK | fs.F_OK);
      } catch (e) {
        console.error(
          chalk.yellow.bold('No .hz/schema.toml file found'));
        return;
      }
      const schemaOptions = schema.processApplyConfig({
        project_name: opts.project_name,
        schema_file: opts.schema_file,
        start_rethinkdb: false,
        connect: '${opts.rdb_host}:${opts.rdb_port}',
        update: true,
        force: false,
      });
      return schema.runApplyCommand(schemaOptions);
    }
  }).then(() => {
    console.log('Starting Horizon...');
    hz_server = start_horizon_server(http_servers, opts);

    return new Promise((resolve, reject) => {
      const timeoutObject = setTimeout(() => {
        reject(new Error('Horizon failed to start after 30 seconds.\n' +
                         'Try running hz serve again with the --debug flag'));
      }, TIMEOUT_30_SECONDS);

      hz_server.ready().then(() => {
        clearTimeout(timeoutObject);
        console.log(chalk.green.bold('🌄 Horizon ready for connections'));
        resolve(hz_server);
      }).catch(reject);
    });
  }).then(() => {
    if (opts.auth) {
      for (const name in opts.auth) {
        const provider = horizon_server.auth[name];
        if (!provider) {
          throw new Error('Unrecognized auth provider "${name}"');
        }
        hz_server.add_auth_provider(provider,
                                    Object.assign({}, { path: name }, opts.auth[name]));
      }
    }
  }).then(() => {
    // Automatically open up index.html in the 'dist' directory only if
    //  '--open' flag specified and an index.html exists in the directory.
    if (opts.open && opts.serve_static) {
      try {
        // Check if index.html exists and readable in serve static_static directory
        fs.accessSync('${opts.serve_static}/index.html', fs.R_OK | fs.F_OK);
        // Determine scheme from options
        const scheme = opts.secure ? 'https://' : 'http://';
        // Open up index.html in default browser
        console.log('Attempting open of index.html in default browser');
        open('${scheme}${opts.bind}:${opts.port}/index.html');
      } catch (open_err) {
        console.log(chalk.red('Error occurred while trying to open ' +
                              '${opts.serve_sta ...
```
- example usage
```shell
...

  return Promise.resolve().then(() => {
    white('Validating current schema version');
    return r.dbList().contains('${project}_internal')
      .branch(true, r.error(internalNotFound))
      .do(() => checkForHzTables)
      .do(() => waitForCollections)
      .run(this.conn)
      .then(() => green(' └── Pre-2.0 schema found'))
      .catch((e) => {
        if (e.msg === internalNotFound) {
          throw new NiceError(e.msg, {
            description: '\
This could happen if you don't have a Horizon app in this database, or if \
you've already migrated this database to the v2.0 format.',
...
```



# <a name="apidoc.module.horizon.version"></a>[module horizon.version](#apidoc.module.horizon.version)

#### <a name="apidoc.element.horizon.version.run"></a>[function <span class="apidocSignatureSpan">horizon.version.</span>run (args)](#apidoc.element.horizon.version.run)
- description and source-code
```javascript
(args) =>
Promise.resolve().then(() => {
  if (args && args.length) {
    throw new Error('create-cert takes no arguments');
  }
  console.info(package_json.version);
})
```
- example usage
```shell
...

  return Promise.resolve().then(() => {
    white('Validating current schema version');
    return r.dbList().contains('${project}_internal')
      .branch(true, r.error(internalNotFound))
      .do(() => checkForHzTables)
      .do(() => waitForCollections)
      .run(this.conn)
      .then(() => green(' └── Pre-2.0 schema found'))
      .catch((e) => {
        if (e.msg === internalNotFound) {
          throw new NiceError(e.msg, {
            description: '\
This could happen if you don't have a Horizon app in this database, or if \
you've already migrated this database to the v2.0 format.',
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
