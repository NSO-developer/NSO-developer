# The NSO Developer organization on GitHub

We have created a public organization on GitHub to ensure we have one common place to share code for all of us working with NSO. 

Since the NSO Developer organization is a public GitHub everyone can fork and read the uploaded code.
By using a pull request everyone can also contribute to existing projects. 

If you want to contribute with a new project, please read the instructions below.

## Licenses
All material on the NSO Developer organization on GitHub is under the [Apache 2.0 license](https://github.com/NSO-developer/NSO-developer/blob/master/LICENSE). 
The license is used to ensure a balance between open contribution and allowing you to use the software as you like to.

The license tells you what rights you have that are provided by the copyright holder. It is important that the contributor fully understands what rights they are
licensing and agrees to them. Sometimes the copyright holder isn't the contributor, such as when the contributor is doing work on behalf of a company.

To ensure that the criteria in the license are met, there is a need for a Developer Certificate of Origin (DCO) sign-off on all contribution. 
More information about that can be found below.

## Contributing a Project on the NSO Developer GitHub
Getting Started
1.	Create an account on github.com
1.	Create your own private repository on github.com
1.	Make sure your project fulfills all the criteria listed below (under “Requirements on your project”).
1.	Send an email to the NSO Developer librarians with a link to your repository (XXX@cisco.com).
1.	You will be asked to add one of the NSO Developer librarians as a collaborator, that person will then MOVE YOUR REPOSITORY to the [NSO Developer GitHub](https://github.com/NSO-developer).
[Read more about the implications here](https://help.github.com/enterprise/2.6/user/articles/about-repository-transfers/).

That’s it! When the move is done, your repository is now part of the NSO developer organization. Keep hacking on your project,
you will still have owner privileges, and as such you can decide to give others write access for example.

Users of your repository can use Issues to report bugs and suggest new features, and Pull Requests to contribute code.

When/if you do not have time to keep your project up to date (fix issues, accept pull requests etc) - please say so. Write a line in the README.md, as well as an email to XXX@cisco.com - we will try to help you find a new maintainer of the code, or retire it from the library if it appears abandoned for a long time.

## Expectations
When using packages from the library you can expect:

*	The code you find provided “as is” and when you use it you get to keep it. If it breaks you get to keep all the pieces.
*	If you extend a project or fix bugs, please contribute back in the form of pull requests.
*	When contributing you can expect:
*	The code you contribute is made available to everyone in source form “as is”.
*	Your code might be used to: teach others about NSO, build new products, provide a starting point for customer projects.
*	At the very minimum your contribution should have a title and a short README.md explaining what it does, see full list of requirements here
*	You are not required to support your contributed code, but please consider pull requests and try to answer questions in the project wiki
*	Only contribute code for which you own the IPR
*	Do not include explicit references to customers (be it customer names, network configuration / templates, or otherwise)

## Requirements on your project
Before your project can be accepted into the NSO Developer organization it needs to fulfill the following criteria.

### Developer Certificate of Origin
When sharing on GitHub you must ensure that your pull request includes a Developer Certification of Origin (DCO). 
The DCO is an attestation attached to every contribution made by every developer. 

```
Developer's Certificate of Origin 1.1

By making a contribution to this project, I certify that:

(a) The contribution was created in whole or in part by me and I
    have the right to submit it under the open source license
    indicated in the file; or

(b) The contribution is based upon previous work that, to the
    best of my knowledge, is covered under an appropriate open
    source license and I have the right under that license to   
    submit that work with modifications, whether created in whole
    or in part by me, under the same open source license (unless
    I am permitted to submit under a different license), as
    Indicated in the file; or

(c) The contribution was provided directly to me by some other
    person who certified (a), (b) or (c) and I have not modified
    it.

(d) I understand and agree that this project and the contribution
    are public and that a record of the contribution (including
    all personal information I submit with it, including my
    sign-off) is maintained indefinitely and may be redistributed
    consistent with this project or the open source license(s)
    involved.
```

In the commit message the contributor simply adds a Signed-off-by statement and thereby agrees to the DCO: 
```
Signed-off-by: N.N. <email@mail.com>
```

### It should be NSO related
Sure, it could be a cool YANG plugin too - but it should at least be relevant to NSO development.

### Naming
Choose a name. A good name. A catchy name, a nerdy name, a happy name - you decide. This is especially important if your contribution is a tool or a reusable library. In that case it doesn’t even have to be descriptive. Better YxT than “YANG Extension Tool”. Don’t pick “generic-tool”, “misc-template”…

If your contribution is more of a demo or example, then a more descriptive name could be in order, perhaps even pre- or postfixed with demo or example. For example: l3-vpn-demo or example-stacked-service.

### README.md
Add a README.md. Your README must include:
*	Brief explanation of what your project does
*	List dependencies (build and runtime, for example compilers, libraries, operating system)
*	Instructions on how to build it
*	If your project contains any copies of code derived from open source you need to explicitly list which projects.

### It must be open
The whole point of the NSO Developer Organization is to share code to the NSO ecosystem, as such we don’t want to make it “private”. However, that means that anyone can access the NSO Developer repositories, which requires us to approve the open access and ensure that no private information is included.

The information in the README.md file will be displayed on the Cisco NSO DevNet site.

### Recommendations
*	Add test cases, and instructions on how to run them. Why not use Lux to automate your tests? NSO uses it!

*	Packaging make one repository for every stand-alone project. But don’t make a lot of small repositories of things that actually belong together, it just makes the organization cluttered and it will be harder to find your project.

*	Naming convention for YANG modules. For a demo or example the module name and namespace does not matter that much (you can use http://example.com/... as namespace). But if your project is a re-usable piece, then consider using the URL of the project the namespace (as in: https://github.com/NSO-developer/PACKAGE-NAME/MODULE-NAME)

*	If you actually make some kind of releases, consider tagging the releases and use a “CHANGES” file / “Release Notes” document
