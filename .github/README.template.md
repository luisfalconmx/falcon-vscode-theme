# ${{ env.REPOSITORY_SLUG }}

#### ${{ env.REPOSITORY_DESCRIPTION }}

![theme-default](https://user-images.githubusercontent.com/57654255/171340854-8d16ffdc-ad42-4295-a5e0-c028e1ca17aa.png)

## Available colours

### Aqua

![theme-aqua](https://user-images.githubusercontent.com/57654255/171340890-a9de6801-4019-4bf9-95d4-b3c76fbef60f.png)

### Blue

![theme-blue](https://user-images.githubusercontent.com/57654255/171340908-c132847a-1f9a-4a72-81d3-fe906f2bfb68.png)

### Green

![theme-green](https://user-images.githubusercontent.com/57654255/171340932-f46fa598-510c-4125-8e6c-f40ad65ba436.png)

### Orange

![theme-orange](https://user-images.githubusercontent.com/57654255/171340943-97c665ca-d509-4de3-80f8-961b3dddfaf9.png)

### Pink

![theme-pink](https://user-images.githubusercontent.com/57654255/171340954-6848134e-275b-46b8-aa87-c867904e951a.png)

### Purple

![theme-purple](https://user-images.githubusercontent.com/57654255/171340975-cfb15391-564b-4266-aa94-8a09c738ce08.png)

### Red

![theme-red](https://user-images.githubusercontent.com/57654255/171340993-858f6be9-1ab6-4f7d-8f4d-4f22947bb9b1.png)

### Sky

![theme-sky](https://user-images.githubusercontent.com/57654255/171341003-b83fb2f6-115f-4418-9a8c-3c6e64afd4d3.png)

### Yellow

![theme-yellow](https://user-images.githubusercontent.com/57654255/171341020-d4a07438-cf02-4716-910a-735f35d210c8.png)

---

## Getting Started

#### First clone the repository from github

```bash
# HTTPS
${{env.REPOSITORY_GITHUB_URL}}.git
```

```bash
# SSH
git@github.com:${{env.REPOSITORY_FULL_NAME}}.git
```

```bash
# GITHUB CLI
gh repo clone ${{env.REPOSITORY_FULL_NAME}}
```

#### Or fork this project clicking in the fork button set in head of this page.

![image](https://user-images.githubusercontent.com/57654255/173211569-3941bbb6-187d-45e9-ac18-d0afd82ea704.png)

If you need help for this step check the next guide:
[https://docs.github.com/en/get-started/quickstart/fork-a-repo](https://docs.github.com/en/get-started/quickstart/fork-a-repo)

#### Set node version with [nvm](https://github.com/nvm-sh/nvm#node-version-manager---) and install dependencies

```
nvm use
npm install
```

#### Finally you can start a local dev server with this command

```
npm start
```

#### Also exists a command for apply code writing rules like indents, semicolons, etc. You can use the following command

```
npm run pretty
```

## Contributing

#### To contribute to the project you need to create a new branch from the main branch

```git
git checkout -b my-new-branch
```

#### Once you complete your project changes can be committed following the standard established by [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/).

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

### Examples

#### Commit message with no body

```
docs: correct spelling of CHANGELOG
```

#### Commit message with scope

```
feat(lang): add Polish language
```

#### Commit message with description and breaking change footer

```
feat: allow provided config object to extend other configs

BREAKING CHANGE: `extends` key in config file is now used for extending other config files
```

If the code passes the tests and the commit message follows the standards set by [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/), you can commit your changes and upload them to the remote repository and you're ready to **create a Pull Request** to the **main branch**.

If you need help to make a pull request, you can consult the following link:

[https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests)

### Linters, Code Formater and other tools

All changes to the project will be validated by creating a commit. These are the tools used to ensure that all code follows the quality standards defined for all contributions:

- [Prettier](https://github.com/prettier/prettier)
- [Husky](https://github.com/typicode/husky)
- [Commitlint](https://github.com/conventional-changelog/commitlint)
- [Lint Staged](https://github.com/okonet/lint-staged)

### Join us in discussions

We use GitHub Discussions to talk about all sorts of topics related to documentation and this site. For example: if you'd like to help troubleshooting a PR, have a great new idea, or want to share something amazing you've learned in our docs, join us in the [discussions](${{env.REPOSITORY_GITHUB_URL}}/discussions).

## Roadmap

Our project roadmap is where you can learn about what features we're working on, what stage they're in, and when we expect to bring them to you. Have any questions or comments about items on the roadmap? Share your feedback in [discussions](${{env.REPOSITORY_GITHUB_URL}}/discussions) section.

Review the project roadmap. Maybe there is something amazing that you can contribute 😉

[${{env.REPOSITORY_GITHUB_URL}}/projects?type=beta](${{env.REPOSITORY_GITHUB_URL}}/projects?type=beta)

## Releases

To create a release it is necessary to prepare the project following these steps

#### Create a new version with tag

```
npm version <version>
```

The above command receives as a parameter a specific version such as 1.4.0 or a version type defined by npm's [semantic versioning](https://docs.npmjs.com/about-semantic-versioning) which will automatically increment the number.

These are the available types that can be used as a parameter:

- **Patch** releases: `1.0` or `1.0.x` or `~1.0.4`
- **Minor** releases: `1` or `1.x` or `^1.0.4`
- **Major** releases: `*` or `x`

### Examples

```
npm version 1.4.0
```

```
npm version minor
```

#### Upload the tag to the remote repository

```
git push origin <tag>
```

Check the complete list of all official releases published:
[${{env.REPOSITORY_GITHUB_URL}}/releases](${{env.REPOSITORY_GITHUB_URL}}/releases)

## License

This project is free and open-source software licensed under the [MIT Licence](${{env.REPOSITORY_LICENSE_URL}}).

Some contents like images, videos, documents and other multimedia files use your own licence and in case required atributtion this is mentioned in any part of this project like in the code or in the documentation.

## Thanks ❤️

Thank you very much for visiting this repository, contributing amazing code and being part of this great community on github.

If you want to support me you can visit my [Github Sponsors Profile](https://github.com/sponsors/${{env.REPOSITORY_OWNER}}). Any support, no matter how small, motivates me to continue creating open source projects and share them with everyone :)