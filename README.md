# action-setup-python-poetry
GitHub action for setting up Python with caching dependencies and Poetry


# Usage

See [action.yml](action.yml).

Basic:
```yaml
steps:
    - name: Setup Python + Poetry
      uses: marns93/action-setup-python-poetry@master
```

With specific versions:
```yaml
steps:
    - name: Setup Python + Poetry
      uses: marns93/action-setup-python-poetry@master
      with:
        python_version: 3.10.0
        poetry_version: 1.1.11
```

With private git repository dependencies:
```yaml
steps:
    - name: Setup Python + Poetry
      uses: marns93/action-setup-python-poetry@master
      with:
        ssh_key: ${{ secrets.SSH_KEY }}
```

