# The NSO Developer space on GitLab & GitHub

NSO-Developer is a public space available on GitLab and GitHub where all of us
working with NSO can publish and share code. Anyone is free to read and use the
code or fork a project and continue development. Contributions are made simple
through Merge/Pull requests and make it possible for anyone to contribute back.

## GitLab vs GitHub
The NSO-Developer space is available both on GitLab and GitHub with the goal to
mirror all projects between the two. Having repos available in both places makes
it possible for users to access code where most convenient for the user.

- If you want to clone a repository, you can grab it from GitLab or GitHub
- If you want to start a new repository you are encouraged to create it on
  GitLab. The repo can be continuously mirrored from GitLab to GitHub.
- If you are the owner of an existing repository on GitHub, talk to an
  administrator to have it moved to GitLab and mirrored back to GitHub. Moving
  to GitLab enables CI functionality.

GitLab and GitHub have virtually the same set of basic functions, like issue
tracking or pull/merge requests for code review. NSO-Developer originally
started on GitHub, which is why the majority of repositories currently have
their home on GitHub. However, GitLab offers the possibility to use the
integrated CI system, thus providing a standardized CI configuration format, yet
setup a custom CI runner (the actual machine running CI jobs). A clear advantage
that in turn makes it possible to run NSO, netsims as well as virtual routers in
CI. The CI system of GitLab together with how it is leveraged in the [NSO in
Docker project](https://gitlab.com/nso-developer/nso-docker/) is why GitLab is
now the preferred location. We encourage anyone starting a new repository to
create it on GitLab. We still keep it available on GitHub by mirroring the
project, making it easy to consume for users.

## Licenses
All material on the NSO-Developer space is under the [Apache 2.0
license](https://github.com/NSO-developer/NSO-developer/blob/master/LICENSE).
The license is used to ensure a balance between open contribution and allowing
anyone to freely use the software without hindrance.

It is important that you, as a contributor, understand the ramifications of the
license and agree to it. Sometimes the copyright holder isn't the contributor,
such as when the contributor is doing work on behalf of a company.

To ensure that the criteria in the license are met, there is a need for a
Developer Certificate of Origin (DCO) sign-off on all contributions.

More information about that can be found below.

## Contributing a Project on the NSO Developer
Getting Started
1. Create an account on gitlab.com
1. Create your own private repository on gitlab.com
1. Make sure your project fulfills all the criteria listed below (under
   “Requirements on your project”).
1. Send an email to the NSO Developer librarians (nso-developer@cisco.com) with
   a link to your repository.
1. You will be added as an outside collaborator to a new repository on the [NSO
   Developer GitHub](https://github.com/NSO-developer) and will be asked to
   contribute your code there.

[Read more about the implications here](https://help.github.com/enterprise/2.6/user/articles/about-repository-transfers/).

That’s it! When the move is done, your repository is now part of the NSO
developer space. Keep hacking on your project, you will still have owner
privileges, and as such you can decide to give others write access for example.

Users of your repository can use **Issues** to report bugs and suggest new features,
and **Merge Requests** to contribute code.

When/if you do not have time to keep your project up to date (fix issues, accept
merge/pull requests etc) - please say so. Write a line in the README, as well as
an email to nso-developer@cisco.com - we will try to help you find a new
maintainer of the code, or retire it from the library if it appears abandoned
for a long time.

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
