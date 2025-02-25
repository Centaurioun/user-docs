# Getting started with Snyk: Free / Team plan

## Introduction&#x20;

In this guide, we’ll look at how you can try a few scans to see the results.&#x20;

Snyk has a number of tools and processes that help secure your entire software development lifecycle. With Snyk, you can scan while you’re coding. You can also monitor code when you’re not working on it. Snyk also provides visibility into issues across your projects with a git repository integration. And Snyk can integrate into CI/CD through integrations, the CLI, or curated containers.

For individuals and small teams, we recommend scanning in the local environment to get started.&#x20;

{% hint style="info" %}
The tool that best serves your tech stack, environment, and workflow will depend on your individual circumstances. See the tech stack implementation guides for more details.
{% endhint %}

To learn more about choosing the integration points within the software development lifecycle that work best for you and your current level of security maturity, see [Ways to integrate Snyk at your company](https://training.snyk.io/courses/ways-to-use-snyk) course in Snyk Training.

### Try out a project

This guide explains how to test a sample or single project in your local development environment or by using the Snyk CLI.

{% hint style="info" %}
Snyk free plan provides limited free tests per month. For unlimited tests, consider a paid plan.
{% endhint %}

#### Create or log into your account

You need a Snyk account to use Snyk functionality, even within your local environment. [Create a free account](../getting-started/quickstart/create-a-snyk-account/) to try out a project. If your organization is already using Snyk, you may be able to log in via single sign-on to be provisioned with a Snyk account (see [Logging in to an existing account](../getting-started/quickstart/create-a-snyk-account/logging-in-to-an-existing-account.md)).

#### Test a project in your local development environment&#x20;

To scan a single project in your local development environment, you need to use a Snyk plugin or extension with your IDE. You also need to authenticate the plugin or extension with your Snyk account, demonstrated in this video.

{% embed url="https://thoughtindustries-1.wistia.com/medias/bva0d7k46b" %}
Install IDE and authenticate to Snyk
{% endembed %}

{% hint style="warning" %}
When authenticating the IDE, you may see a warning about scanning folders you trust. Because Snyk is executing code, such as invoking the package manager to get dependency information, you’ll need to trust the folder you’re scanning to continue.
{% endhint %}

A scan with the Snyk IDE plugin or extension in a local project surfaces information about open source package issues, including fix advice.

{% embed url="https://thoughtindustries-1.wistia.com/medias/bny3j0ywui" %}
Review open source dependency issues video
{% endembed %}

Scanning with the Snyk IDE plugin or extension in a local project also surfaces information about code issues, including example fixes.

{% embed url="https://thoughtindustries-1.wistia.com/medias/fazwzk6oi3" %}
Review code issues video
{% endembed %}

#### Test a project with the Snyk CLI

Some package managers rely on context from the local environment, so testing in the local environment or as part of the CI/CD pipeline provides the most accurate results.

You need to [install the Snyk CLI](../snyk-cli/install-the-snyk-cli.md). Once installed, you need to authenticate it to your Snyk account, demonstrated in this video.

{% embed url="https://thoughtindustries-1.wistia.com/medias/ava7rrg7al" %}
Authenticate CLI video
{% endembed %}

A scan with [**Snyk test**](../products/snyk-open-source/use-snyk-open-source-from-the-cli/) surfaces information about open source package issues, including fix advice, demonstrated in this video.&#x20;

{% embed url="https://thoughtindustries-1.wistia.com/medias/b8vrvtmnbu" %}
Snyk test video
{% endembed %}

A scan with [**Snyk code test** ](../products/snyk-code/cli-for-snyk-code/)runs a Static Code Analysis test on the code in that project, and returns the list of detected vulnerability issues, general information about the test, and a summary of the test findings.

A scan with [**Snyk container test**](../scan-containers/snyk-cli-for-container-security/) returns a list of vulnerabilities in the container image, along with recommendations for upgrading the base image for one that is more secure. &#x20;

A scan with [**Snyk iac test**](../scan-cloud-deployment/snyk-infrastructure-as-code/snyk-cli-for-infrastructure-as-code/) returns advice on how to resolve discovered issues in your Infrastructure as Code files.

### What’s next?

* When you are ready to start scanning more applications, read the [Preparing for implementation guide: Free / Team plan](preparing-for-implementation-free-team-plan.md).&#x20;
* To get specific recommendations for your tech stack, read the guide specific to your language.
* If you decide you want to expand Snyk usage throughout your business, and involve more teams in Snyk, read the [Getting started with Snyk: Enterprise plan](getting-started-with-snyk-enterprise-plan.md).
