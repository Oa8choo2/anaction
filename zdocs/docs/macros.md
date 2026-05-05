# Testfile for macros

Since v40 (dd 20260511 22) zensical has support for macros.

See <https://zensical.org/docs/setup/extensions/macros/>

## replace a variable

the zensical.toml contains following lines:

```text
[project.markdown_extensions.zensical.extensions.macros]
on_error_fail = true
on_undefined = "strict"
include_yaml = ["variables.yml"]
```

the variables.yml contains the variable,  
this file is in the root of this zensical project  
i.e. in the zdocs dir (the dir where the zensical.toml is)

```yaml
computer: "name of a computer"
```

a computer such as: {{ computer }}.

```django
a computer such as: {{ computer }}.
```

---

Now it is {{ now() }}, now means at time this file was build

```jinja
Now it is {{ now() }}
```

```django
two_days_ago -> {% now 'utc' - 'days=2', '%Y-%m-%dT%H:%M:%SZ' %}
```

   now('%Y-%m-%dT%H:%M:%SZ' ... seems not to work

---

## set a variable and display it

```django
{% set x = 42 %}
{{ x }}
```

{% set x = 42 %}
Here you see the variable: - {{ x }} -

## git variables

Committed on {{ git.date }} by {{ git.author }}, build on {{ now() }}
