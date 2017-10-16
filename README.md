# tango-schema

[![Join the chat at https://gitter.im/5gtango/tango-schema](https://badges.gitter.im/5gtango/tango-schema.svg)](https://gitter.im/5gtango/tango-schema?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

The schema files for the various descriptors used by 5GTANGO as well as some examples and tests. The schema files in this repository serve as ground truth for the whole 5GTANGO project. Thus, every tool and sub-project should be able to parse and handle the latest versions of these files (or - once available - tagged versions in corresponding branches).

The 5GTANGO schemas are a fork of the SONATA NFV schemas which have been developed in the 5GPPP project SONATA ([http://sonata-nfv.eu](http://sonata-nfv.eu)).

The schema files are written in JSON-Schema Draft-04.

## Development

To contribute to the development of the 5GTANGO schema files, you may use the very same development workflow as for any other 5GTANGO Github project. That is, you have to fork the repository and create pull requests. Moreover, all discussions regarding the 5GTANGO schemas take place on GitHub, and NOT on the wiki.

### Contributing

You may contribute to the schema files similar to other 5GTANGO (sub-) projects, i.e. by creating pull requests. However, since changes in the schema file may affect several other tools and projects, the pull requests might be discussed on the mailing list before it is merged to the master branch.

### Integration with Jenkins

The repository is integrated with Jenkins. Thus, every pull request is checked automatically. The Jenkins job validates all the JSON and YAML files in the repository to be a valid JSON/YAML format. Moreover, Jenkins executes all files named 'test_*.sh' that reside in */test/ directories automatically. Thus, it is quite easy to add new tests. Just write a corresponding bash script. Tests are considered successful when they return with exit code 0, and to be a failure otherwise.

### Useful Tools

There are some useful tools that support working the JSON and YAML files.

- http://jsonviewer.stack.hu/ A nice JSON editor
- http://yamltojson.com/ Convert YAML to JSON
- http://jsontoyaml.com/ Convert JSON to YAML
- http://jsonschemalint.com/draft4/#/ Write JSON-Schema documents and validate JSON
- http://jsonschema.net/#/ Create JSON-Schema from JSON documents

## License

The 5GTANGO schemata for the VNF descriptor as well as the NS descriptor is published under Apache 2.0 license. Please see the LICENSE file for more details.

## Useful Links

- http://json-schema.org/ The general JSON-Schema standard

---
#### Lead Developers

The following lead developers are responsible for this repository and have admin rights. They can, for example, merge pull requests.

- Manuel Peuster (@mpeuster)
- Stefan Schneider (@StefanUPB)

#### Feedback-Chanel

* Please use the GitHub issues to report bugs.
