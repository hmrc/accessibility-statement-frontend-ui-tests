# accessibility-statement-frontend-ui-tests

[accessibility-statement-frontend](https://github.com/hmrc/accessibility-statement-frontend) UI journey tests.

## Pre-requisites

### Services

Start `ACCESSIBILITY_STATEMENT_FRONTEND` services as follows:

```bash
sm2 --start ACCESSIBILITY_STATEMENT_FRONTEND
```

## Tests

Run tests as follows:

* Argument `<browser>` must be `chrome`, `edge`, or `firefox`.
* Argument `<environment>` must be `local`, `dev`, `qa` or `staging`.

```bash
sbt clean -Dbrowser="<browser>" -Denvironment="<environment>" "testOnly uk.gov.hmrc.ui.specs.*" testReport
```

## Scalafmt

Check all project files are formatted as expected as follows:

```bash
sbt scalafmtCheckAll scalafmtCheck
```

Format `*.sbt` and `project/*.scala` files as follows:

```bash
sbt scalafmtSbt
```

Format all project files as follows:

```bash
sbt scalafmtAll
```

## License

This code is open source software licensed under the [Apache 2.0 License]("http://www.apache.org/licenses/LICENSE-2.0.html").
