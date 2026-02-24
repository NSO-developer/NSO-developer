# The NSO Developer Space on GitHub (Primary) & GitLab (Legacy Mirror)

**NSO-Developer** is a public community space where anyone working with NSO can share, explore, and collaborate on projects. All repositories are open for reading, cloning, and forking, and contributions are welcomed through Pull Requests.

We aim to make collaboration simple, transparent, and accessible for the entire NSO ecosystem.

## Repository Hosting Policy

The NSO-Developer organization is available on both GitHub and GitLab. However:

**GitHub is now the primary and only location for creating new NSO-Developer repositories.**  
GitLab is maintained only as a legacy mirror for existing projects and is **no longer used for new project creation.**

## License

All material in the NSO-Developer space is released under the **Apache 2.0 License**:  
https://github.com/NSO-developer/NSO-developer/blob/master/LICENSE

This license ensures:

- open collaboration
- freedom to use the software
- protection for contributors

Contributors must understand and agree to the license terms. In cases where work is done on behalf of an employer, the employer may hold copyright.

To comply with licensing requirements, **all contributions must include a Developer Certificate of Origin (DCO) sign-off.**

## Contributing a Project to NSO-Developer

### Getting Started

1. Create a GitHub account if you don’t already have one.
2. Prepare your project locally or in your own GitHub repository.
3. Ensure your project satisfies the requirements listed below.
4. Email **nso-developer@cisco.com** with:
   - repository link
   - project description
   - maintainer contact information
5. The NSO-Developer librarians will review your submission.
6. If accepted, your project will be transferred or added to the  
   https://github.com/NSO-developer organization.

After onboarding:

- You retain maintainer privileges.
- You can grant collaborators access.
- Community members can submit Pull Requests and Issues.

## Maintenance Expectations

If you are no longer able to maintain your project:

1. Add a note in the repository README indicating maintenance status.
2. Email **nso-developer@cisco.com**

The librarians may:

- help find a new maintainer, or
- archive the repository if it appears inactive long-term.

## Project Requirements

Projects submitted to NSO-Developer should:

- be relevant to NSO users or developers
- include documentation
- build and run as described
- follow licensing rules
- accept community collaboration

Projects that do not meet these expectations may be declined or later archived.

## Community Philosophy

NSO-Developer exists to foster collaboration, learning, and sharing across the NSO community. Whether you’re publishing a new tool, improving an existing project, or contributing fixes, your participation helps everyone.

We’re glad you’re here, and we’re excited to see what you build.

## Expectations
When using packages from the library you can expect:

- The code you find provided “as is” and when you use it you get to keep it. If
  it breaks you get to keep all the pieces.
- If you extend a project or fix bugs, please contribute back in the form of
  merge/pull requests.

When contributing you can expect:
- The code you contribute is made available to everyone in source form “as is”.
- Your code might be used to: teach others about NSO, build new products,
  provide a starting point for customer projects.
- At the very minimum your contribution should have a title and a short
  README.md explaining what it does, see full list of requirements here
- You are not required to support your contributed code, but please consider
  merge/pull requests and try to respond to issues and feedback
- Only contribute code for which you own the IPR
- Do not include explicit references to customers (be it customer names, network
  configuration / templates, or otherwise)

## Requirements on your project
Before your project can be accepted as a repository of the NSO Developer it
needs to fulfill the following criteria.

### Developer Certificate of Origin
#### Signed-off
For code published on NSO-developer, every commit needs to be signed-off (git
commit –s) by the contributor that he or she has the right to submit it.

The “-s” flag adds a line with the text 'Signed-off-by' followed by the same
email address as the contributor. E.g.

```
My commit message

Signed-off-by Aron Aronsson <aron.aronsson@example.com>
```

It is important that the git config user.name and user.email is configured
correctly.

[user]
        name = Aron Aronsson
        email = aron.aronsson@example.com

#### What is signed-off
In short you are signing off that you have the right to submit the code to the
NSO-Developer space, and that you understand that it will be public. The full
text can found at [developercertificate.org](www.developercertificate.org) and
below:

```
Developer Certificate of Origin
Version 1.1

Copyright (C) 2004, 2006 The Linux Foundation and its contributors.
1 Letterman Drive
Suite D4700
San Francisco, CA, 94129

Everyone is permitted to copy and distribute verbatim copies of this
license document, but changing it is not allowed.


Developer's Certificate of Origin 1.1

By making a contribution to this project, I certify that:

(a) The contribution was created in whole or in part by me and I
    have the right to submit it under the open source license
    indicated in the file; or

(b) The contribution is based upon previous work that, to the best
    of my knowledge, is covered under an appropriate open source
    license and I have the right under that license to submit that
    work with modifications, whether created in whole or in part
    by me, under the same open source license (unless I am
    permitted to submit under a different license), as indicated
    in the file; or

(c) The contribution was provided directly to me by some other
    person who certified (a), (b) or (c) and I have not modified
    it.

(d) I understand and agree that this project and the contribution
    are public and that a record of the contribution (including all
    personal information I submit with it, including my sign-off) is
    maintained indefinitely and may be redistributed consistent with
    this project or the open source license(s) involved.
```


### It should be NSO related
Sure, it could be a cool YANG plugin too - but it should at least be relevant to
NSO development.

### Naming
Choose a name. A good name. A catchy name, a nerdy name, a happy name - you
decide. This is especially important if your contribution is a tool or a
reusable library. In that case it doesn’t even have to be descriptive. Better
YxT than “YANG Extension Tool”. Don’t pick “generic-tool”, “misc-template”…

If your contribution is more of a demo or example, then a more descriptive name
could be in order, perhaps even pre- or postfixed with demo or example. For
example: l3-vpn-demo or example-stacked-service.

### Repository Description
Be sure to set the description of the repository. While the name might be
catchy, do try to use the description to describe what the package does.

Is it just an example? Or a reusable library ready for use? Is it an NSO package
or a peripheral utility? What does it do? How does it help someone else?

### README.md
Add a README.md. Your README must include:
* Brief explanation of what your project does
* List dependencies (build and runtime, for example compilers, libraries,
  operating system)
* Instructions on how to build it
* If your project contains any copies of code derived from open source you need
  to explicitly list which projects.

### LICENSE
Add a LICENSE file so that the license is kept with the repository, we suggest
using Apache 2.0 license. This makes it clear for anyone how the code can be
used, modified and distributed.

### It must be open
The whole point of the NSO Developer space is to share code to the NSO
ecosystem, as such we don’t want to make it “private”. However, that means that
anyone can access the NSO Developer repositories, which requires us to approve
the open access and ensure that no private information is included.

The information in the README.md file will be displayed on the Cisco NSO DevNet
site.

### Recommendations
- Add test cases, and instructions on how to run them. Why not use Lux to
  automate your tests? NSO uses it!
- Packaging make one repository for every stand-alone project. But don’t make a
  lot of small repositories of things that actually belong together, it just
  makes the space cluttered and it will be harder to find your project.
- Naming convention for YANG modules. For a demo or example the module name and
  namespace does not matter that much (you can use example.com/... as
  namespace). But if your project is a re-usable piece, then consider using the
  URL of the project the namespace (as in:
  github.com/NSO-developer/PACKAGE-NAME/MODULE-NAME)
- If you actually make some kind of releases, consider tagging the releases and
  use a “CHANGES” file / “Release Notes” document

## Link to GitLab & GitHub

- [NSO-Developer on GitLab](https://gitlab.com/nso-developer) 
- [NSO-Developer on GitHub](https://github.com/nso-developer) 
