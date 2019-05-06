# Terminalizer Redacted

## Project Outline

Terminalizer is a great tool, but I found that I needed to mask certain strings from the output found in the scripted Yaml output files.

The aim of this project is to provide a simple way of applying filters with regexes, in an easy-to-configure Yaml file.

An example of strings to filter will be the hostname of the prompt, file timestamps, Guids, IP addresses, etc... 

### Setup and Configuration

In order to use the app, run the command;

```
go get -u hook-s3c/terminalizer-redacted
```

Generate the default global config by issuing the command;

```
terminalizer-redacted config global
```

This will drop the default config file (.redacted.yml) in \$HOME/.config/terminalizer/

### Usage

Using the app;

```
terminalizer-redacted redact
```

The app will parse the output in a temporary file and then prompt the user to preview the output via Terminalizer.

The app will take your configuration setup from either the global config or a local one.
You can specify profiles, as explained in the Configuration file section below.

#### Overriding global config

You can generate a per-directory config by issuing the command;

```
terminalizer-redacted config local
```


#### Configuration file

As you can see, the format is simple to follow;

```

```

#### Greetz

As always, big shout out to my vap0r family, Thugcrowd, r0bl0xgang - y33t!
