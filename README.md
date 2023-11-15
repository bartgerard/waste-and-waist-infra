# waste-and-waist-infra

Waste &amp; Waist Infra

## Getting Started

### Install Scoop (Windows only)

#### Windows

1. Open a PowerShell terminal.
2. Run:

```
$ Set-ExecutionPolicy RemoteSigned -Scope CurrentUser # Optional: Needed to run a remote script the first time

$ irm get.scoop.sh | iex
```

### Install Brew (Mac OS X only)

#### Mac OS X

1. Open a terminal.
2. Run:

```
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### Install Okteto

#### Windows

```
$ scoop install okteto
```

#### Mac OS X

```
$ brew install okteto
```

### Okteto

#### Configuration with Okteto Cloud

The first thing you need to do is configure Okteto CLI to use Okteto Cloud.
To do this, run the command below:

```
$ okteto context use https://cloud.okteto.com
```

#### Launch

```
$ git clone <YOUR_REPOSITORY>
$ cd <your_repo_directory>

$ okteto context cloud.okteto.com

$ okteto up
```

### Microsoft SQL Server

1. Database > + > Data Source > Microsoft SQL Server

| property | value                      |
|----------|----------------------------|
| user     | sa                         |
| password | Admin123                   |
| url      | jdbc:sqlserver://localhost |

## Elasticsearch

1. Chrome > Extensions > Elasticvue
2. Elasticvue > Add cluster

| property | value                 |
|----------|-----------------------|
| url      | http://localhost:9200 |

