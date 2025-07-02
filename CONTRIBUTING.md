# Contributing

When contributing to this repository, please first discuss the change you wish to make via [issue](https://github.com/humansbehindkeyboards/charts/issues), email, or any other method with the owners of this repository before making a change. 

Please note we have a code of conduct, please follow it in all your interactions with the project.

## Branch naming convention

| Instance | Branch Name | Description |
|----------|:-----------:|-------------|
| Stable | `main` | Accepts merges from Working and Hotfixes |
| Working | `dev` | Accepts merges from Features/Issues and Hotfixes |
| Feature/Issue | `feat/feature-name` or `fix/bug-name` | Always branch off HEAD of Working |
| Hotfix | `hotfix/hotfix-name` | Always branch off Stable |

## Content

### Container Images

All the Container Images must be stored in the `containers/` directory, for instance:

```diff
  .
  ├── .github
  ├── containers/
+ │   ├── hello-world/
  │   │   ├── ...
  │   │   └── Dockerfile
  │   └── ...
  ├── charts/
  │   ├── hello-world/
  │   │   ├── templates
  │   │   ├── Chart.yaml
  │   │   └── values.yaml
  │   └── ...
  ├── README.md
  ├── LICENSE
  ├── CONTRIBUTING.md
- └── my-container-image/
      └── ...
```

- `hello-world` container image placed in `containers/` it's in the right location
- `my-container-image` placed in the root it's in the wrong location

### Helm Charts

All the Helm Charts must be stored in the `charts/` directory, for instance:

```diff
  .
  ├── .github
  ├── containers/
  │   ├── hello-world/
  │   │   ├── ...
  │   │   └── Dockerfile
  │   └── ...
  ├── charts/
+ │   ├── hello-world/
  │   │   ├── templates
  │   │   ├── Chart.yaml
  │   │   └── values.yaml
  │   └── ...
  ├── README.md
  ├── LICENSE
  ├── CONTRIBUTING.md
- └── my-helm-chart/
      └── ...
```

- `hello-world` chart placed in `charts/` it's in the right location
- `my-helm-chart` placed in the root it's in the wrong location

## Merge Request Process

1. Ensure any install or build dependencies/values are removed before the end of the layer when doing a build.
2. Update the README.md with details of changes to the interface, this includes e.g., new parameters.
3. Increase the version numbers in any examples files and the README.md to the new version that this Merge Request would represent. The versioning scheme we use is [SemVer](http://semver.org/).
4. You may merge the Merge Request in once you have the sign-off of another developer, or if you do not have permission to do that, you may request the reviewer to merge it for you.

> Be careful, do not squash multiple commits into one, we prefer to have the full commit history of our codebase.

# Code of Conduct

## Our Pledge

We as members, contributors, and leaders pledge to make participation in our community a harassment-free experience for everyone, regardless of age, body size, visible or invisible disability, ethnicity, sex characteristics, gender identity and expression, level of experience, education, socio-economic status, nationality, personal appearance, race, caste, color, religion, or sexual identity and orientation.

We pledge to act and interact in ways that contribute to an open, welcoming, diverse, inclusive, and healthy community.

## Attribution

This Code of Conduct is adapted from the Contributor Covenant, version 2.1, available [here](https://www.contributor-covenant.org/version/2/1/code_of_conduct/).
