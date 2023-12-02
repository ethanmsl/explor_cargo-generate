# Liquid Mustache's

## Cargo-Generate Builtins

### Authors: {{authors}}

> this will be filled in by a function borrowed from Cargo's source code, that determines your information from Cargo's configuration. It will either be on the form username <email> or just plain username.

### Project-Name: {{project-name}}

> this is supplied by either passing the --name flag to the command or working with the interactive CLI to supply a name.

### Crate_Name: {{crate_name}}

> the snake_case_version of project-name

### Crate_Type: {{crate_type}}

> this is supplied by either passing the --bin or --lib flag to the command line, contains either bin or lib, --bin is the default

### OS-Arch: {{os-arch}}

- contains the current operating system and architecture ex: linux-x86_64

### UserName: {{username}}

> this will be filled in by a function borrowed from Cargo's source code, that determines your information from Cargo's configuration.

### Within_Cargo_Project (bool): {{within_cargo_project}}

> A boolean with the value true if the template is being expanded inside a Cargo project. It's a simple matter of whether Cargo.toml is present in any parent folder.

### Is_Init (bool): {{is_init}}

> A boolean that reflects the value of the --init parameter of cargo-generate.

## Not Builtin, Not defined in `cargo-generate.toml`

- Bops: {{bops}}
- made up: {{made-up}}

## Not Builtin, ARE defined in `cargo-generate.toml`

- Ramalama: {{ramalama}}
- HyperVisor: {{ hypervisor }}
- Network_Enabled: {{ network_enabled }}
