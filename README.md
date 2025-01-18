# README

Two ways to create a new python project:

- create project by copier:

```sh
copier copy --trust https://github.com/fluent-qa/fluentqa-pytpl.git my-project
```

- create project by UV, because UV is so fast

```sh
mkdir my-project && cd my-project
uv pip install --source git+https://github.com/fluent-qa/fluentqa-pytpl.git

```
