# Contributing

Thank you for your interest in contributing to Arcturus, there are several ways you can contribute and make this project
more awesome, please see below:

## Reporting an Issue

If you believe you have found an issue with the code please do not hesitate to file an issue
in [GitHub](https://github.com/arcturusvn/arcturus-soma-build/issues). When filing the issue please describe the problem with the
maximum level of detail and the steps to reproduce the problem, including information about your environment.

You can also open an issue requesting for help or doing a question, and it's also a good way of contributing since other
users might be in a similar position.

Please note we have a code of conduct, please follow it in all your interactions with the project.

## Code Contributions

When contributing to this repository, it is generally a good idea to discuss the change with the
owners before investing a lot of time coding.

**The process could be:**

1. Open an issue explaining the improvement or fix you want to add
2. [Fork the project](https://github.com/arcturusvn/arcturus-soma-build/fork_select)
3. Code it in your fork
4. Submit a merge request

**Don't forget to add tests**, make sure that they all pass!

## Setup IDE & Coding Style

This project uses Google's style code: https://google.github.io/styleguide/javaguide.html

**Step 1**: Install plugin `google-java-format` and enable for this project

**Step 2**: Download config style for your IDE
> **IntelliJ IDE**: [intellij-java-google-style.xml](https://github.com/google/styleguide/blob/gh-pages/intellij-java-google-style.xml)
>
> **Eclipse IDE**:  [eclipse-java-google-style.xml](https://github.com/google/styleguide/blob/gh-pages/eclipse-java-google-style.xml)

**Step 3**: Import config file to IDE
> **IntelliJ IDE**: Go to `File` → `Settings` → `Editor` → `Code Style`. There click on the icon
> next
> to the `Scheme` section. There, click on the `Import Scheme`
>
> **Eclipse IDE**: Updating ...

## Help with Git

Once the repository is forked, you should track the upstream (original) one using the following
command:

```shell
git remote add upstream git@github.com:arcturusvn/arcturus-soma-build.git
```

Then you should check out to `build` branch (Ex: 1.0.x)
```shell
git checkout [major.minor.x]
```

And you should create your own branch:

```shell
git checkout -b <prefix>/<micro-title>
```

Once your changes are done (`git commit -am '<descriptive-message>'`), get the upstream changes:

```shell
git checkout [major.minor.x]
git pull --rebase origin [major.minor.x]
git pull --rebase upstream [major.minor.x]
git checkout <your-branch>
git rebase [major.minor.x]
```

Finally, publish your changes:

```shell
git push -f origin <your-branch>
```

You should be now ready to make a merge request.