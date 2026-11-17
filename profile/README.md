## Ubicity
Your automation tools handle individual components. Ubicity handles
the system: one declarative model for the full lifecycle of complex,
multi-vendor systems, from cloud and data center to edge and the plant
floor. Terraform, Ansible, Helm and Kubernetes become tools the
orchestrator drives, not tools it replaces.

Ubicity is built on OASIS TOSCA 2.0, the current version of the
standard. Ubicity contributes to and runs the TOSCA community's v2.0
conformance tests. Chris Lauwers, Ubicity's CEO, chairs the OASIS TOSCA
Technical Committee, and Ubicity is a member of the Open Process
Automation Forum (OPAF) and Margo.
### Open Source: TOSCA Parser and Validator
[`tosca-core`](https://github.com/ubicity-corp/tosca-core): The open
reference for parsing and validating TOSCA 2.0, under the Apache 2.0
license. It checks service templates and profiles against TOSCA's
rules before anything is deployed, from Python or from the command
line, and also accepts the TOSCA Simple Profile in YAML 1.3. Install it
from [PyPI](https://pypi.org/project/tosca-core/); issues and pull
requests are welcome.
### Model Translators
- [`any2tosca`](https://github.com/ubicity-corp/any2tosca): Convert
  JSON Schema files to TOSCA profiles.
- [`oas2tosca`](https://github.com/ubicity-corp/oas2tosca): Convert
  Swagger definitions to TOSCA data types.
- [`yang2tosca`](https://github.com/ubicity-corp/yang2tosca): A pyang
  plugin that converts YANG modules to TOSCA data type definitions.
### Ubicity Orchestrator
The Ubicity Orchestrator is the production runtime built on
`tosca-core`. It deploys a TOSCA service template and manages it for
the rest of its life: updates, scaling, failure recovery and
decommissioning. Domain knowledge lives in TOSCA profiles rather than
in the engine, so supporting a new domain means writing a profile, not
changing the orchestrator.

In process automation, the orchestrator deploys and manages
multi-vendor control systems modeled with O-PAS Part 9
(Orchestration), the part of the Open Process Automation Standard that
is built on TOSCA.

The orchestrator is commercial software. Evaluation licenses are
available; see [ubicity.com](https://ubicity.com).
